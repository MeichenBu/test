<template>
  <div>
    <div class= "message"> {{msg}} </div>
    <div class = "button" @click = "click()">button</div>
  </div>
    </template>


<script>
export default {
  data () {
    return {
      msg: 0
    }
  },

  methods: {
    click () {
      this.msg += 1
    }
  }
}
</script>

<style scoped>
.message {
 font-size: 30px;
 text-align: center;
 width:100%；
}

.userinfo {
  display: flex;
  flex-direction: column;
  align-items: center;
}

.userinfo-avatar {
  width: 128rpx;
  height: 128rpx;
  margin: 20rpx;
  border-radius: 50%;
}

.userinfo-nickname {
  color: #aaa;
}

.usermotto {
  margin-top: 150px;
}

.form-control {
  display: block;
  padding: 0 12px;
  margin-bottom: 5px;
  border: 1px solid #ccc;
}
.all{
  width:7.5rem;
  height:1rem;
  background-color:blue;
}
.all:after{
  display:block;
  content:'';
  clear:both;
}
.left{
  float:left;
  width:3rem;
  height:1rem;
  background-color:red;
}

.right{
  float:left;
  width:4.5rem;
  height:1rem;
  background-color:green;
}
</style>
