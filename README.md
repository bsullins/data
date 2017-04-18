# data
data sets for my online courses

## How to get data from github api
1 - Get ``sha`` of file
```
 ~ $ curl https://api.github.com/repos/bsullins/data/contents/MonthlySales.csv
{
  "name": "MonthlySales.csv",
  "path": "MonthlySales.csv",
  "sha": "7ef73f68ac207eb7405ebae8ee6e94e2b41134e3",
  "size": 82,
  "url": "https://api.github.com/repos/bsullins/data/contents/MonthlySales.csv?ref=master",
  "html_url": "https://github.com/bsullins/data/blob/master/MonthlySales.csv",
  "git_url": "https://api.github.com/repos/bsullins/data/git/blobs/7ef73f68ac207eb7405ebae8ee6e94e2b41134e3",
  "download_url": "https://raw.githubusercontent.com/bsullins/data/master/MonthlySales.csv",
  "type": "file",
  "content": "bW9udGgsc2FsZXMNMTAsMTAwDTIwLDEzMA0zMCwyNTANNDAsMzAwDTUwLDI2\nNQ02MCwyMjUNNzAsMTgwDTgwLDEyMA05MCwxNDUNMTAwLDEzMA==\n",
  "encoding": "base64",
  "_links": {
    "self": "https://api.github.com/repos/bsullins/data/contents/MonthlySales.csv?ref=master",
    "git": "https://api.github.com/repos/bsullins/data/git/blobs/7ef73f68ac207eb7405ebae8ee6e94e2b41134e3",
    "html": "https://github.com/bsullins/data/blob/master/MonthlySales.csv"
  }
}
```

2 - Get contents of file using ``sha``
```
~ $ curl https://api.github.com/repos/bsullins/data/git/blobs/7ef73f68ac207eb7405ebae8ee6e94e2b41134e3
{
  "sha": "7ef73f68ac207eb7405ebae8ee6e94e2b41134e3",
  "size": 82,
  "url": "https://api.github.com/repos/bsullins/data/git/blobs/7ef73f68ac207eb7405ebae8ee6e94e2b41134e3",
  "content": "bW9udGgsc2FsZXMNMTAsMTAwDTIwLDEzMA0zMCwyNTANNDAsMzAwDTUwLDI2\nNQ02MCwyMjUNNzAsMTgwDTgwLDEyMA05MCwxNDUNMTAwLDEzMA==\n",
  "encoding": "base64"
}
```

3 - Decode contents
