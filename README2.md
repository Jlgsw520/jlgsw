<!-- 单行输入框 -->
<input type="text" id="inputText" placeholder="请输入密码">
<button onclick="getInputValue()">提交</button>
<p id="showResult"></p >

<script>
// 获取输入内容并展示
function getInputValue() {
    const input = document.getElementById('inputText');
    const result = document.getElementById('showResult');
    if (input.value.trim() === '') {
        result.textContent = "输入不能为空！";
        return;
    }
    result.textContent = `密码是：${input.value}`;
    input.value = ''; // 清空输入框
}
</script>
