# redis-slack

## test
```shell
# connect
$ redis-cli -p 6359                                                                                                                                                                      ✔ 

# test
$ bf.add test 11
(integer) 1

$ bf.madd test 22 33

$ bf.exists test  11
(integer) 1

$ bf.exists test  44
(integer) 0
```


## other
https://juejin.cn/post/7135840044547309598