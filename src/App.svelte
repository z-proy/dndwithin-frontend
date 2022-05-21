<script lang="ts">
	import { Button, Form, Input, Collapsible, Checkbox  } from 'spaper'
	import AttrBlock from './components/AttrBlock.svelte';
	import CharHeader from './components/CharHeader.svelte';
	import Navbar from "./lib/Navbar.svelte"
	import CharSearch from './components/CharSearch.svelte';
import AttrRow from './components/AttrRow.svelte';
import Table from 'spaper/components/Table.svelte';


	const data = [
	{"Skill":"Spellcraft", "Modifier": "19"},
    {"Skill":"Bluff", "Modifier": "17"},
	{"Skill":"Stealth", "Modifier": "14"},
	{"Skill":"Knowledge (Arcana)", "Modifier": "11"},
	{"Skill":"Sleight of Hand", "Modifier": "10"},
	{"Skill":"Disguise", "Modifier": "7"},
	{"Skill":"Knowledge (Planes)", "Modifier": "6"},
    {"Skill":"Concentration", "Modifier": "5"},
    {"Skill":"Escape Artist", "Modifier": "5"},
    {"Skill":"Intimidate", "Modifier": "5"},
    {"Skill":"Knowledge (History)", "Modifier": "5"},
    {"Skill":"Knowledge (Local)", "Modifier": "5"},
    {"Skill":"Knowledge (Religion and Nobility)", "Modifier": "5"},
	{"Skill":"Diplomacy", "Modifier": "4"},
	{"Skill":"Search", "Modifier": "4"},
	{"Skill":"Use Rope", "Modifier": "3"},
	{"Skill":"Sense Motive", "Modifier": "2"},
	{"Skill":"Perform", "Modifier": "1"},
    {"Skill":"Perception", "Modifier": "0"},
    {"Skill":"Spot", "Modifier": "0"},
    {"Skill":"Survival", "Modifier": "0"},
	{"Skill":"Athletics", "Modifier": "-1"}
]
</script>

<main>
	<div>
		<link rel="stylesheet" href="https://unpkg.com/papercss@1.8.3/dist/paper.min.css">
		<div>
			<Navbar charName="Anluryn"/>
		</div>
		<br/>
		<br/>
		<br/>
		<div class="charHeader">
			<CharHeader Name="Anluryn"/>
			<CharSearch />
		</div>
		<div class="child-borders statsMods">
			<div class="border-primary">
				<h3>Attributes and Abilities</h3>
				<AttrRow />
				<Table {data} />
			</div>
		</div>
		<div class="child-borders statsMods">
			<div class="border-primary">
				<h3>Spellbook: Dungeon</h3>
				<Collapsible label="test">
				<Button size="small">Cast</Button>
				</Collapsible>
			</div>
		</div>
	</div>
	
</main>

<style>
	main {
		background-image: url("https://www.photos-public-domain.com/wp-content/uploads/2011/02/white-parchment-paper-texture.jpg");
		background-size: cover;
		display: grid;
	}
	h3 {
		text-align: center;
		margin-top: 5px;
		margin-bottom: 5px;
	}

	.charHeader {
		text-align: center;
	}
	.statsMods {
		width: 550px;
	}
/*	
	@media (min-width: 600px) {
		main {
			max-width: none;
		}
		h1 {
			color: blueviolet;
		}
	}
*/
</style>