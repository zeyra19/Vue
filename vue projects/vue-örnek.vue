// <html kodlarını burada, ara yüzü burada tasarla
<template>
    <div>
        <h1>{{message}}</h1>
    </div>
</template>

// ara yüz fonksiyonlarını oluştur
<script>
    export default {
        data() {
            return {
                message: "Vue ilk örnek"
            };
        }
    };
</script>

// ara yüze burada şekil ver
// eğer style scoped olmazsa css özellikleri tüm bileşenlerde çalışır
<style scoped>
h1 {
    color: blue
}
</style>