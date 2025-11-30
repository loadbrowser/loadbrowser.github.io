<!DOCTYPE html>
<html lang="ru">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Попап Скачать</title>
<style>
  body { font-family: Arial, sans-serif; margin:0; padding:0; }
  .button { padding: 10px 20px; margin: 10px; background:#007bff; color:#fff; border:none; cursor:pointer; border-radius:4px; }
  .modal { display:none; position:fixed; top:0; left:0; width:100%; height:100%; background:rgba(0,0,0,0.5); justify-content:center; align-items:center; }
  .modal-content { background:#fff; padding:20px; border-radius:8px; width:90%; max-width:400px; text-align:center; position:relative; }
  #modalDownload { padding:10px 20px; background:#28a745; color:#fff; border:none; cursor:pointer; border-radius:4px; }
  .close { position:absolute; top:10px; right:15px; font-size:20px; cursor:pointer; }
</style>
</head>
<body>

<!-- Кнопки для примера -->
<button class="button" data-title="Приложение A" data-desc="Описание приложения A" data-href="fileA.zip">Скачать A</button>
<button class="button" data-title="Приложение B" data-desc="Описание приложения B" data-href="fileB.zip">Скачать B</button>

<!-- Попап -->
<div id="modal" class="modal">
  <div class="modal-content">
    <span class="close">&times;</span>
    <h2 id="modalTitle">Скачать приложение</h2>
    <div id="modalDescription" style="margin-bottom:20px;"></div>
    <a id="modalDownload" href="#" download>Скачать</a>
  </div>
</div>

<script>
  const modal = document.getElementById('modal');
  const modalDownload = document.getElementById('modalDownload');
  const modalTitle = document.getElementById('modalTitle');
  const modalDescription = document.getElementById('modalDescription');
  const closeBtn = document.querySelector('.close');

  document.querySelectorAll('.button').forEach(btn => {
    btn.addEventListener('click', () => {
      const title = btn.getAttribute('data-title');
      const desc = btn.getAttribute('data-desc');
      const href = btn.getAttribute('data-href');

      modalTitle.textContent = title;
      modalDescription.textContent = desc;
      modalDownload.setAttribute('href', href);

      modal.style.display = 'flex';
    });
  });

  closeBtn.addEventListener('click', () => { modal.style.display = 'none'; });
  window.addEventListener('click', (e) => { if(e.target === modal) modal.style.display = 'none'; });
</script>

</body>
</html>
