// seçilmiş form varsa ve seçilen formda ism girilmemişse uyarı fırlat
<p v-if="selectedForm && !username">
    Bir kullanıcı adı girin
</p>

// seçilmiş form yoksa ve seçilen formda ism girilmemişse uyarı fırlat
<p>
    Dosya seçilmedi veya kullanıcı adı yok
</p>