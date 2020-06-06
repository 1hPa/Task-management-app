<templete>
  <div class="container">
    <div class="item">
      <input type="text" name="title">
    </div>
    <div class="item">
      <input type="text" name="period">
    </div>
    <div class="item">
      <textarea name="detail"></textarea>
    </div>
    <div class="item">
      <button>作成</button>
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
