<script>
  import { t } from 'svelte-i18n';

  import Button from '../../components/Button.svelte';

  export let account;
  export let deleteAccount;
  export let cancel;
</script>

<div>
  <p class="text-white font-bold mb-4 text-lg">{$t('settings.modal.delete')} {account.label}?</p>
  <p class="text-white mb-4">{$t('settings.modal.notice')}</p>
  <div class="flex justify-end gap-2">
    <Button on:click={cancel}>{$t('settings.modal.cancel')}</Button>
    <Button on:click={deleteAccount} color="red">{$t('settings.modal.delete')}</Button>
  </div>
</div>
