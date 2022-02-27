<template>
<div id="container">
  <input type="checkbox" id="read-more">
  <label for="read-more"></label>
  
  <div id="content">
    <p style="text-align=center">邓小平演讲稿</p>
    <p>“文革”后，逐渐形成了以邓小平为核心的党的第二代领导集体。面对“文革”后濒于崩溃的经济和混乱不堪的社会状况，新的中央领导集体在继承了毛泽东的经验，并深刻总结了毛泽东的教训的基础上，提出了“制度问题更带有根本性、全局性、稳定性和长期性”，制度建设重于其它建设，注重制度建设成为以邓小平为核心的党的第二代领导集体的基本治国方略。</p>
    <p>在实践中，邓小平渐认识到，法制是加强和巩固制度建设的可靠保障，从而把民主与法制结合到一起，开创了邓小平理论的新境界。</p>
    <p>建设社会主义民主政治是把民主制度化、法律化。民主与法制密不可分，邓小平很早就认识到了这一点。因此在研究邓小平的法制思想时，我们不能抛开他早期的民主政治思想。1941年，邓小平在中央北方局出版的《党的生活》杂志上发表的《党与抗日民主政权建设》一文中，开宗明义称“三三制政权的实质是民主。”</p>
    <p>这种民主的含义是“必然在政权中反映出不同的利益，不同的党派立场，不同党派阶级的民主政治斗争。”共产党的领导和政治优势，“更基本的是从民主政治斗争中去取得。”</p>

  </div>
</div>
</template>

<script>
export default {
  name: 'HelloWorld',
}
</script>

<style scoped>
body {
  font-family: Helvetica;
  font-size: 15px;
  background-color: #eee;
  margin: 40px;
}

#container {
  position: relative;
  width: 300px;
  margin: auto;
  overflow: hidden;
  border-radius: 6px;
}

#content {
  padding: 30px;
  background-color: #fff;
  height: 400px;
  font-size: 1.2rem;
  line-height: 1.5rem;
  color: #333;
  text-indent:2em;
}

p {
  margin: 0 0 30px;
}

#read-more {
  display: none;
}

#read-more + label {
  display: block;
  position: absolute;
  width: 100%;
  height: 150px;
  bottom: 0;
  left: 0;
  background-image: linear-gradient(to bottom, rgba(255, 255, 255, 0) 0%, #fff 70%);
  pointer-events: none;
}

#read-more + label::after {
  content: 'Read More';
  display: inline-block;
  position: absolute;
  bottom: 20px;
  left: 50%;
  transform: translateX(-50%);
  background-color: #333;
  font-size: 1.2rem;
  color: #fff;
  padding: 8px 14px;
  border-radius: 4px;
  box-shadow: 0px 2px 2px rgba(0, 0, 0, .2);
  cursor: pointer;
  pointer-events: auto;
}

#read-more + label:hover::after {
  background-color: #000;
}

#read-more:checked ~ #content {
  height: auto;
}

#read-more:checked + label {
  display: none;
}
</style>
