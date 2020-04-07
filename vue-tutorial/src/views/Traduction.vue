<template>
  <div class="traduction">
    <img  src="../assets/1_Classic_Logo_Transparent.png" class="rounded mx-auto d-block"  alt="Responsive image">
    <TraductionComponent msg1="traduction "/>
            <form action="/traduire" method="POST" enctype="multipart/form-data" class="main-form">

    <div class="select-col">
		<div class="select-col-ins">
  <select  id="selectlang">
                        <option >Allemand</option>	
                        <option  selected="" class="EN">Anglais</option>	

                        </select>
		</div>
    </div>
    <div class="select-col">
		<div class="select-col-ins">
  <select  id="selectspeciality">
			<option selected="">speciality</option>
                <option>generaliste</option>
                </select>
		</div>
	</div>
     <div class="select-col">
		<div class="select-col-ins">
  <select  id="selectspeciality">
			<option selected="">context</option>
                <option>context</option>
                </select>
		</div>
	</div>
    <button v-on:click: class="btn confirmer">confirmer</button>
            </form>
             <table class="table table-hover">
                <thead>
                  <tr>
                    <th scope="col">Français</th>
                    <th scope="col">Anglais</th>
                    <th scope="col">translate : {{langname}}</th>
                  </tr>
                </thead>
                <tbody>
<tr>
    
			<td align="left" >Français</td>
			<td align="left">Englais</td>
			<td align="right">
		<input v-modele="" type="textarea" ip="ip" rows="5" style="overflow:auto" size="30%" >
			</td>
		</tr>

                </tbody>
              </table>
              <a href="#" class="previous">&laquo; Previous</a>
              <a href="/traduire" class="next">Next &raquo;</a>
              <button v-on:click: class="btn">valide</button>
</div>
</template>

<script>
// @ is an alias to /src
import TraductionComponent from '@/components/TraductionComponent.vue'

export default {

  name: 'Traduction',
  components: {
    TraductionComponent
  }
}
</script>
