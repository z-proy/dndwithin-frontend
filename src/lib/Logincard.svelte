<script lang="ts">
	import { Button, Form, Input } from 'spaper'
</script>

<main>
	<div class="card" style="width: 20rem;">
		<div class="card-body">
		  <h4 class="card-title">D&D-Within</h4>
		  <Form>
			<Input placeholder="Username" block/> 
			<Input type="password" placeholder="Password" block/> 
		  </Form>
		  <Button>Login</Button>
		</div>
	  </div>
</main>

<style>
    main {
        text-align: center;
    }
</style>