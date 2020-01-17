<template>
  <div id="app">
    <div id="nav">
      <router-link to="/">Home</router-link> |
      <router-link to="/about">About</router-link>
    </div>
  <router-view/>
  </div>
</template>

<style lang="less">
#app {
  padding: 0;
  margin: 0;
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  width: 100%;
  height: 100vh;
  background: #0068B5;/* 为较旧的或者不支持的浏览器设置备用属性 */
  background: -moz-linear-gradient(left, #b53697 0%, #e18f3e 100%);/**/
  background: -webkit-gradient(linear, left, right, color-stop(0%, #b53697), color-stop(100%, #e18f3e));/**/
  background: -webkit-linear-gradient(left, #b53697 0%, #e18f3e 100%);/**/
  background: -o-linear-gradient(left, #b53697 0%, #e18f3e 100%);/**/
  background: -ms-linear-gradient(left, #b53697 0%, #e18f3e 100%);/**/
  background: linear-gradient(to right, #b53697 0%, #e18f3e 100%);/*用线性渐变创建图像*/
  filter: progid:DXImageTransform.Microsoft.gradient( startColorstr='#0068B5', endColorstr='#7CAFE1', GradientType=0);/* ie6 - ie8*/
}

#nav {
  padding: 30px;
  background-color: rgba(0,0,0,0.55);
  a {
    font-weight: bold;
    color: #8d8d8d;

    &.router-link-exact-active {
      color: #42b983;
    }
  }
}
</style>
