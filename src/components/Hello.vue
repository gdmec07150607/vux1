<template>
  <div>
    <span class ="title">
      欢迎登陆
    </span>
    <diver>Vue Vux</diver>
    <Group>
      <XInput title="账号" v-model='account' placeholder='账号' type='text'>
      </XInput>
    </Group>
    <x-input title="密码" v-model="password" placeholder="密码" type="password"/>
    <XButton type="primary" action-type="button">登陆</XButton>
  </div>
</template>

<script>
import { Divider, Group, XInput, XButton } from 'vux'
export default {
  components: {
    Divider,
    Group,
    XInput,
    XButton
  },
  data () {
    return {
      account: '',
      password: ''
    }
  }
}
</script>
