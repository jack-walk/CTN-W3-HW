<!--
@component
WhyCare.svelte — Description of why readers should care about this article

An infobox with key reasons readers should care about this article.
Features three bullet points containing key insights.

USAGE EXAMPLE:
<WhyCare>
  r1="This is an example."
  r2="This is another attempt."
  r3="I really hope this works."
</WhyCare>
-->

<script>
  let { r1, r2, r3 } = $props();
</script>

<ul class="infobox">
<div class="whyCareHead">Why does this matter?</div>
  <li class="reason">{r1}</li>
  <li class="reason">{r2}</li>
  <li class="reason">{r3}</li>
</ul>

<style>
  .infobox {
    margin: 2rem 0;
    padding: 1rem;
    padding-left: 1.5rem;
    border-left: 4px solid var(--color-accent);
    background-color: var(--color-light-gray);
  }

  .reason{
    margin-bottom: 0.75rem;
    font-size: 1rem;
    line-height: 1.6;
    margin-left: 3rem;
  }

  .whyCareHead{
    font-size: 1.25rem;
    font-weight: bold;
    margin-bottom: 1rem;
    color: var(--color-dark);
  }
</style>