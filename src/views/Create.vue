<template>
  <div class="create">
        <form  @submit.prevent="addContato(form)">
            <h1>Cadastrar contato</h1>
                    <h2>Novo Contato</h2>
                    <div class="field" >
                        <label for="name">Nome</label>
                        <input type="text" v-model="form.name" id="name" name="name" placeholder="Ex:Lucas"  required="required">
                    </div>
                    <div class="field">
                        <label for="tel">Telefone</label>
                        <input type="tel" v-model="form.tel" id="tel" placeholder="Ex:55-99999999" maxlength="12"  required="required">
                    </div>
                    <div class="field">
                        <label for="e-mail">E-mail</label>
                        <input type="text" v-model="form.email" id="email" name="email" placeholder="Ex:Lucas@hotmail.com"  required="required">
                    </div>
                   
            <button>Salvar</button>
            <div id="conts">   
                    <h1>CONTATOS</h1>                   
                        <hr/>
                        <h2>{{form.name}}</h2>
                        <h2>{{form.tel}}</h2>
                        <h2>{{form.email}}</h2>
                        <hr/>
                </div>   
       </form>
       
  </div>
</template>

<script>
// @ is an alias to /src

export default {
  name: "Contato",
  data:() =>({
      form: { 
          name:'',
          tel:'',
          email:''
        }
  }),
  methods: {
      addContato(form) {
          form.id = Date.now()
          console.log(this.form)
      }
  }
};
</script>

