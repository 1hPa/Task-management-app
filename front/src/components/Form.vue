<templete>
  <div class="container">
    <div class="item">
      <input type="text" name="title" v-model="inputTitle">
    </div>
    <div class="item">
      <input type="text" name="period" v-model="inputPeriod">
    </div>
    <div class="item">
      <textarea name="detail" v-model="inputDetail"></textarea>
    </div>
    <div class="item">
      <button v-on:click="creatTask">作成</button>
    </div>
  </div>
</templete>

<script>
export default{
    date(){
        return{
          inputTitle: "",
          inputPeriod: "",
          inputDetail: ""
        };
    },
    methods:{
        creatTask(){
            //タスクを生成する処理
        }
    }
};
</script>
