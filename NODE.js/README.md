### 홈페이지 구현

강의링크 : https://www.inflearn.com/course/lecture?courseSlug=web2-node-js&unitId=12638

조건문을 통해 url 별로 홈페이지 구현



![image-20230313221508308](README.assets/image-20230313221508308.png)





---

### 파일목록 알아내기

##### 하고자 하는것 : data를 수정할때 , 파일의 여러부분을 수정해야한다.

##### 해결하고자 하는 방법 : data directory가 수정됬을때 nodejs를 통해 알아낼 수 있는가 

#####                                           -> fs.readdir





![image-20230313223251510](README.assets/image-20230313223251510.png)

사용코드

```javascript
var testFolder = './data';
var fs = require('fs');

fs.readdir(testFolder, function(error,fileList){
  console.log(fileList);
});
```

---

