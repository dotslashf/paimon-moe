<script>
  import { t } from 'svelte-i18n';
  import { mdiInformation } from '@mdi/js';
  import Icon from './Icon.svelte';
</script>

<div>
  <div class="flex items-center mb-4">
    <span class="text-gray-400 mr-2">
      <Icon path={mdiInformation} />
    </span>
    <h1 class="font-display text-gray-400 text-lg">{$t('calculator.guide.clickToMaximize')}</h1>
  </div>
  <div class="bg-background p-2 rounded-xl mb-2">
    <h1 class="font-display text-white text-lg">{$t('calculator.guide.howToWeapon')}</h1>
    <a href="/images/calculator-weapon.png" target="__blank">
      <img src="/images/calculator-weapon.png" alt="how to use calculator weapon" />
    </a>
  </div>
  <div class="bg-background p-2 rounded-xl mb-2 mt-8">
    <h1 class="font-display text-white text-lg">{$t('calculator.guide.howToCharacter')}</h1>
    <a href="/images/calculator-character.png" target="__blank">
      <img src="/images/calculator-character.png" alt="how to use calculator character" />
    </a>
  </div>
</div>
