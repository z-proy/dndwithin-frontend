<script>
    import AttrBlock from "./AttrBlock.svelte";
</script>

<main>
    <div class="attrDisplayRow">
        <AttrBlock Name="Str" Value="8" Bonus="5"/>
        <AttrBlock Name="Dex" Value="17" Bonus="5"/>
        <AttrBlock Name="Con" Value="12" Bonus="5"/>
        <AttrBlock Name="Int" Value="23" Bonus="5"/>
        <AttrBlock Name="Wis" Value="10" Bonus="5"/>
        <AttrBlock Name="Cha" Value="13" Bonus="5"/>
    </div>
</main>


<style>
	.attrDisplayRow{
		display: flex;
		flex-direction: row;
		flex-wrap: wrap;
		padding-top: 0px;
	}
</style>