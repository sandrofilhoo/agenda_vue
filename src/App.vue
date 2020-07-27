<template>
  <div id="app">
    <div id="nav">
      <router-link to="/">Home</router-link> |
      <router-link to="/Create">Novo contato</router-link> 
     
    </div>
    <router-view />
  </div>
</template>

<style >
header{
  margin-left: 574px;
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  
  color: #000;
  
}

#nav {
  padding: 30px;
  text-align: center;
}

#nav a {
  font-weight: bold;
  color: #000;
  text-decoration: none;
}

#nav a.router-link-exact-active {
  color: #ff9d00;
}

#create{
    width: 90%;
    max-width: 1100px;
    margin: 0;
}
form{
    background-color: white;
    margin: 20px auto;

    padding: 44px;
    border-radius: 8px;
    max-width: 730px;
    font-family: Ubuntu;
    
}
form h1{
    font-size: 36px;
}
form fieldset{
    margin-top: 44px;
    border: 0;

}
form legend{
    margin-bottom: 40px;
    display: flex;
    align-items: center;
    justify-content: space-between;

    width: 100%;
}
form legend h2{
    font-size: 24px;
}
form .field{
    flex: 1;
    display: flex;
    flex-direction: column;
    margin-bottom: 24px;
}
form .fiel-group{
    display: flex;
}
form input,
form select{
    background-color: #f0f0f5;
    border: 0;
    padding: 16px 24px;
    font-size: 16px;
    border-radius: 8px;
}
form label{
    font-size: 14px;
    margin-bottom: 8px;
    flex-direction: column;
}
form .fiel-group .field + .field{
    margin-left: 24px;
}
form button{
    width: 256px;
    height: 56px;
    background-color: #ff9d00;
    border-radius: 8px;
    color: white;
    font-weight: bold;
    font-size: 16px;
    border: 0;
    margin-top: 40px;
    transition: background-color 400ms;
}
form button:hover{
    background-color: #c85103;
}
form fieldset legend h1{
  margin-left: 580px;
}

</style>