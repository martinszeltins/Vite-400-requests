<template>
    Hello world<br>
    Why is this app making 400 HTTP requests to date-fns from dev server?
</template>

<script>
import eo from 'date-fns/locale/eo'
import { formatWithOptions } from 'date-fns/fp'

export default {
    setup() {
        const dateToString = formatWithOptions({ locale: eo }, 'yyyy-mm-dd')
    }
}
</script>
