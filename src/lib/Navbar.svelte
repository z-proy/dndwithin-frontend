<script lang="ts">
    import { Modal, Button, Form, Select } from 'spaper'
    let showModal = false;
    export let charName: string
    let nameButtonValue = charName
</script>
<main>
<nav class="border fixed split-nav">
<div class="nav-brand">
    <h3>D&D-Within</h3>
    </div>
    <div class="collapsible">
      <input id="collapsible1" type="checkbox" name="collapsible1">
        <label for="collapsible1">
          <div class="bar1"></div>
          <div class="bar2"></div>
          <div class="bar3"></div>
          <div class="bar4"></div>
          <div class="bar5"></div>
        </label>
    <div class="collapsible-body">
        <ul class="inline">
            <li><b>Spells</b></li>
            <li><b>Spellbooks</b></li>
            <li>Dossier: <Button size="small" type="secondary" on:click={() => showModal = true}><b>{nameButtonValue}</b></Button></li>
            <Modal bind:active={showModal}>
                <Form>
                    <Select label="Available Dossiers" bind:value={nameButtonValue}>
                        <option value="Anluryn">Anluryn</option>
                        <option value="Cyrus">Cyrus</option>
                    </Select>
                </Form>
            </Modal>
            </ul>
          </div>
        </div>
      </nav>
</main>
<style></style>