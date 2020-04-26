<script>
  import { onMount } from 'svelte'

  /**
   *  Direct Chat Link from tawk.to dashboard
   *  https://tawk.to/chat/{propertyId}/{chatId}
   * /

  /**
   * Property ID
   * @type {string}
   */
  export let propertyId = ''

  /**
   * Chat id
   * @type {string}
   */
  export let chatId = 'default'

  onMount(() => {
    // Widget code from dashboard
    const Tawk_API = Tawk_API || {},
      Tawk_LoadStart = new Date()
    ;(function() {
      var s1 = document.createElement('script'),
        s0 = document.getElementsByTagName('script')[0]
      s1.async = true
      s1.src = `https://embed.tawk.to/${propertyId}/${chatId}`
      s1.charset = 'UTF-8'
      s1.setAttribute('crossorigin', '*')
      s0.parentNode.insertBefore(s1, s0)
    })()
  })
</script>
