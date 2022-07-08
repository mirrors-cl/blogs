<template>
  <div class="backimgclass">
    <div class="box">
      <h2>Login</h2>
      <div class="input-box">
        <label>账号</label>
        <input type="text" />
      </div>
      <div class="input-box">
        <label>密码</label>
        <input type="password" />
      </div>
      <div class="btn-box">
        <a href="#">忘记密码？</a>
        <div>
          <button>登陆</button>
          <button>注册</button>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "logIn",
  data() {
    return {};
  },
};
</script>

<style>
.backimgclass {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  width: 100%;
  height: 100%;
  background-image: url(../assets/image/backimg.png);
  background-size: 100% 100%;
}
.box {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  /* background-image: url(../assets/image/32545_9453221544.webp); */
  /* background-size: 100% 100%; */
  background: rgba(50,50,50,0.2);
  backdrop-filter: blur(10px);
  height: 350px;
  width: 350px;
  border-radius: 8px;
}
.box .input-box{
  margin-bottom: 10px;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: start;
}
.box .input-box > label{
color: rgba(5, 0, 0, 0.9);
}
.box .input-box > input {
  color: rgba(255, 255, 255, 0.9);
  font-size: 14px;
  height: 35px;
  width: 250px;
  background: rgba(255, 255, 255, 0.3);
  border: 1px solid rgba(255, 255, 255, 0.5);
  border-radius: 5px;
  transition: 0.2s;
  outline: none;
}
.box .input-box > input:focus {
  border:  1px solid rgba(255, 255, 255, 0.8);
}
.box .btn-box {
  width: 250px;
  display: flex;
  flex-direction: column;
  align-items: start;
}
.box .btn-box > a {
  outline: none;
  display: block;
  width: 250px;
  color: rgba(255, 255, 255, 0.9);
  font-size: 13px;
  text-align: end;  /* 文本对齐方式 */
  text-decoration:none;
}
.box .btn-box > a:hover {
  color: rgba(255, 255, 255, 1);
}
.box .btn-box > div {
  margin-top: 10px;
  display: flex;
  justify-content: center;
  align-items: center;
}
.box .btn-box > div > button {
  outline: none;
  margin-top: 10px;
  display: block;
  font-size: 14px;
  border-radius: 5px;
  transform: 0.2s;
  cursor: pointer;
}
.box .btn-box > div > button:nth-of-type(1) {
  width: 120px;
  height: 35px;
  border: 1px solid rgba(192, 119, 91, 0.7);
  background: rgba(192, 119, 91, 0.5);
}
.box .btn-box > div > button:nth-of-type(2) {
  margin-left: 10px;
   width: 120px;
  height: 35px;
  border: 1px solid rgba(192, 119, 91, 0.7);
  background: rgba(192, 119, 91, 0.5);
}
.box .btn-box > div >button:hover{
  border: 1px solid rgba(251, 128, 71, 0.7);
  background: rgba(251, 128, 71, 0.5);
}
</style>