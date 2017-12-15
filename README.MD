#install
```bash
npm html5-storage
```

by commonJS
```bash
let storageUtil = require("html5-storage");
```
by Script tag
```bash
<script src="../index.js"></script>
<script>
    storageUtil.setLocalStorage("name","1");
    console.log(storageUtil.getLocalStorage("name"));
</script>
```
#API
```bash
/**
 * 根据键值获取sessionStorage
 * @param key 键
 * @returns 失败false,成功对象
 */
storageUtil.getSession (key)


/**
 * 设置sessionStorage
 * @param key 键
 * @param value 值   String或者JSON或者ARRAY
 * @returns {boolean}
 */
storageUtil.setSession(key , value)


/**
 * 移除sessionStorage
 * @param key
 * @returns {boolean}
 */
storageUtil.removeSession(key)


/**
 * 清空所有Session
 * @returns {boolean}
 */
storageUtil.clearSession()


/**
 * 根据键值获取localStorage
 * @param key 键
 * @returns 失败false,成功对象
 */
storageUtil.getLocalStorage (key)


/**
 * 设置localStorage
 * @param key 键
 * @param value 值   String或者JSON或者ARRAY
 * @returns {boolean}
 */
storageUtil.setLocalStorage(key , value)


/**
 * 移除localStorage
 * @param key
 * @returns {boolean}
 */
storageUtil.removeLocalStorage(key)


/**
 * 清空所有localStorage
 * @returns {boolean}
 */
storageUtil.clearLocalStorage()
```
 
