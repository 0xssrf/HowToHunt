
# Another Method

### Tools You Will Need for this method.
* [https://github.com/tomnomnom/meg](https://github.com/tomnomnom/meg)
* [https://github.com/tomnomnom/gf](https://github.com/tomnomnom/gf)
* [https://github.com/projectdiscovery/subfinder](https://github.com/projectdiscovery/subfinder)
* [https://github.com/tomnomnom/assetfinder](https://github.com/tomnomnom/assetfinder)
* [https://github.com/Edu4rdSHL/findomain](https://github.com/Edu4rdSHL/findomain)
* [https://github.com/projectdiscovery/httpx](https://github.com/projectdiscovery/httpx)
         
### Steps
```
1) Find Domains with the help of subfinder,assetfinder,findomain i.e , subfinder -d target.com | tee -a hosts1 , findomain -t target.com | tee -a hosts1 , assetfinder --subs-only target.com |tee -a hosts1 .
2) Then cat hosts1 | sort -u | tee -a hosts2 and then cat hosts2 | httpx | tee -a hosts .
3) Navigate through terminal where hosts file is located  echo "/" > paths
4) Then type meg -v
5) After the completion of process type gf cors.
6) All the urls with Access-Control-Allow will be displayed.  
```


