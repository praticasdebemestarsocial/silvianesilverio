---
layout: cv
permalink: /cv/
title: Currículo
nav: true
nav_order: 5
cv_pdf: # você pode adicionar um link para baixar o seu PDF aqui depois
cv_format: rendercv
description: Este é o meu currículo completo, contendo todas as minhas qualificações, cursos e experiências profissionais.
toc:
  sidebar: left
---

<style>
/* Torna a foto de perfil redonda */
img[src*='foto_perfil.jpg'] {
    border-radius: 50% !important;
    width: 150px !important;
    height: 150px !important;
    object-fit: cover !important;
    margin: 0 auto;
    display: block;
    box-shadow: 0px 4px 10px rgba(0, 0, 0, 0.1);
}
</style>

<script>
// Traduz os termos em inglês do layout padrão do currículo
document.addEventListener("DOMContentLoaded", function() {
    // Substituição direta no HTML para ser à prova de quebras de linha
    const contentDiv = document.querySelector('.post');
    if (contentDiv) {
        let html = contentDiv.innerHTML;
        html = html.replace(/>\s*Contact Information\s*</g, '>Contato<');
        html = html.replace(/>\s*Name\s*</g, '>Nome<');
        html = html.replace(/>\s*Professional\s*<br>\s*Title\s*</g, '>Profissão<');
        html = html.replace(/>\s*Professional Title\s*</g, '>Profissão<');
        html = html.replace(/>\s*Education\s*</g, '>Educação (Graduação e Pós)<');
        html = html.replace(/>\s*Experience\s*</g, '>Experiência Profissional<');
        html = html.replace(/>\s*Certificates\s*</g, '>Cursos de Formação e Eventos<');
        html = html.replace(/>\s*Awards\s*</g, '>Congressos e Seminários<');
        contentDiv.innerHTML = html;
    }
});
</script>
