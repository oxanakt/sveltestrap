<script>
  import Dropdown from './Dropdown.svelte';

  let className = '';
  export { className as class };
  export let active = false;
  export let addonType = false;
  export let direction = 'down';
  export let disabled = false;
  export let dropup = false;
  export let group = false;
  export let inNavbar = false;
  export let isOpen = false;
  export let nav = false;
  export let setActiveFromChild = false;
  export let size = '';
  export let toggle = undefined;
</script>

<Dropdown
  {...$$restProps}
  {group}
  class={className}
  {disabled}
  {direction}
  {isOpen}
  {nav}
  {active}
  {addonType}
  {size}
  {toggle}
  {inNavbar}
  {setActiveFromChild}
  {dropup}
  on:click>
  <slot />
</Dropdown>
