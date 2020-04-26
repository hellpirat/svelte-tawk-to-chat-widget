<script>
  import { onMount } from 'svelte'

  /**
   *  Direct Chat Link from tawk.to dashboard
   *  https://tawk.to/chat/{tawkToPropertyId}/{tawkToChatId}
   * /

  /**
   * Property ID
   * @type {string}
   */
  export let tawkToPropertyId = ''

  /**
   * Chat id
   * @type {string}
   */
  export let tawkToChatId = 'default'

  onMount(() => {
    // Widget code from dashboard
    const Tawk_API = Tawk_API || {},
      Tawk_LoadStart = new Date()
    ;(function() {
      var s1 = document.createElement('script'),
        s0 = document.getElementsByTagName('script')[0]
      s1.async = true
      s1.src = `https://embed.tawk.to/${tawkToPropertyId}/${tawkToChatId}`
      s1.charset = 'UTF-8'
      s1.setAttribute('crossorigin', '*')
      s0.parentNode.insertBefore(s1, s0)
    })()
  })
</script>
