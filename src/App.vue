<template>
 <table class="table is-bordered is-striped is-narrow is-hoverable is-fullwidth">
      <thead>
        <tr>
          <th >One</th>
          <th>Two</th>
        </tr>
      </thead>
      <tbody>
       
        <tr v-for="item in items" :key="item.number" >
          <td>{{item.string}}</td>
          <td>{{item.number}}</td>
        </tr>
      </tbody>
    </table>
</template>

<script>
 

export default {
  name: 'App',
   data:()=>({
     items:[
        {string:'five',number:5},
       {string:'one',number:1},
       {string:'two',number:2},
        {string:'four',number:4},
         {string:'three',number:3},
     ]
   })
}
</script>
