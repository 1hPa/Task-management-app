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
import api from "@/api";

export default{
    date(){
        return{
          inputTitle: "",
          inputPeriod: "",
          inputDetail: ""
        };
    },
    methods:{
        asnyc creatTask(){
            const result = await api.post("/tasks",{
                title: this.inputTiltle,
                period: this.inputPeriod,
                detail: this.inputDetail
                });
            console.log(result);
        }
    }
};
</script>
