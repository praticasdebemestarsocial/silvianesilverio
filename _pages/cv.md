---
layout: cv
permalink: /cv/
title: Currículo
nav: true
nav_order: 5
cv_pdf: 
cv_format: rendercv
description: Este é o meu currículo completo, contendo todas as minhas qualificações, cursos e experiências profissionais.
toc:
  sidebar: left
---

<style>
  .post table {
    table-layout: fixed;
    width: 100%;
  }
  .post td, .post th, .cv table, .cv td {
    word-break: break-word;
    overflow-wrap: break-word;
  }
  .protected-cert {
    position: relative;
    display: inline-block;
    user-select: none;
    -webkit-user-select: none;
  }
  .protected-cert img {
    user-drag: none;
    -webkit-user-drag: none;
  }
  .protected-cert::after {
    content: 'USO EXCLUSIVO - PROIBIDA CÓPIA';
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%) rotate(-30deg);
    font-size: clamp(0.8rem, 2.5vw, 1.8rem);
    color: rgba(255, 255, 255, 0.9);
    background-color: rgba(180, 0, 0, 0.75);
    padding: 8px 15px;
    border-radius: 6px;
    pointer-events: none;
    white-space: nowrap;
    font-weight: bold;
    box-shadow: 0 4px 6px rgba(0,0,0,0.4);
    text-shadow: 1px 1px 2px rgba(0,0,0,0.8);
    z-index: 10;
  }
</style>
<script>
  document.addEventListener('contextmenu', function(e) {
    if (e.target.tagName === 'IMG') {
      e.preventDefault();
      alert('⚠️ AVISO: A cópia ou reprodução destes documentos é terminantemente proibida.');
    }
  });
</script>

<div id="cv-custom-footer" style="display: none; padding-top: 30px;">
    <hr>
    <div style="background-color: #ffebee; color: #b71c1c; padding: 15px; border-radius: 8px; border: 1px solid #ef9a9a; text-align: center; margin-top: 40px; margin-bottom: 40px; font-weight: 500;">
      ⚠️ <strong>AVISO LEGAL:</strong> Todos os documentos apresentados nesta página são de propriedade exclusiva, apenas para consulta. Qualquer reprodução, alteração ou uso indevido será considerado crime e sujeito às medidas legais cabíveis.
    </div>

    <br>
    <h3 class="mb-4 text-center">Encontros com Personalidades da Iridologia</h3>
    <p class="text-center mb-4">Momentos especiais e trocas de conhecimento com grandes referências mundiais.</p>

    <div class="row mb-5">
        <!-- Substitua 'sua_foto_1.jpg' e o texto abaixo quando fizer o upload das imagens para assets/img/ -->
        <div class="col-sm-4 mt-3 mt-md-0 text-center">
            <img src="{{ '/assets/img/template_error.png' | relative_url }}" class="img-fluid rounded z-depth-1 mb-2" alt="Encontro 1" style="object-fit: cover; height: 250px; width: 100%;">
            <p class="text-muted font-weight-bold mt-2">Dr. Bernard Jensen (Exemplo)</p>
        </div>
        
        <div class="col-sm-4 mt-3 mt-md-0 text-center">
            <img src="{{ '/assets/img/template_error.png' | relative_url }}" class="img-fluid rounded z-depth-1 mb-2" alt="Encontro 2" style="object-fit: cover; height: 250px; width: 100%;">
            <p class="text-muted font-weight-bold mt-2">Dr. David J. Pesek (Exemplo)</p>
        </div>
        
        <div class="col-sm-4 mt-3 mt-md-0 text-center">
            <img src="{{ '/assets/img/template_error.png' | relative_url }}" class="img-fluid rounded z-depth-1 mb-2" alt="Encontro 3" style="object-fit: cover; height: 250px; width: 100%;">
            <p class="text-muted font-weight-bold mt-2">Ellen Tart-Jensen (Exemplo)</p>
        </div>
    </div>
</div>

<script>
  document.addEventListener("DOMContentLoaded", function() {
      // O layout do al-folio coloca o conteúdo renderizado do yaml dentro da tag <article> ou <div class="post">
      const postContent = document.querySelector('article') || document.querySelector('.post');
      const cvFooter = document.getElementById('cv-custom-footer');
      if (postContent && cvFooter) {
          // Move o footer customizado para o final da página após o conteúdo do currículo
          postContent.appendChild(cvFooter);
          cvFooter.style.display = 'block';
      }
  });
</script>
