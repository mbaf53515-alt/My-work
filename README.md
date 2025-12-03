# My-work
Many people come look my creation 
<!DOCTYPE html>
<html lang="fr">
	<head>
	<meta charset="UTF-8"/>
<meta name="viewport" content="width=device-width,initial-scale=1" />
		<title>Mon premier site</title>
		<style>
			body{
				margin: 0;
				height: 100vh;
				background:linear-gradient(145deg, #ff0055, #5500ff, #00ccff);
				transition: background 0.5 ease;
				}
				body:hover{
					background: linear-gradient(90deg, #5500ff, #00ccff, #ff0055);
				}
:root{
    --card-bg:#fff;
    --accent:#ff476f;
    --muted:#666;
    --glass: rgba(255,255,255,0.7);
  }
  body{
    margin:0;
    font-family:system-ui,Segoe UI,Roboto,"Helvetica Neue",Arial;
    background: linear-gradient(135deg, #0f172a, #0b3a5a);
    min-height:100vh;
    color:#111;
    display:flex;
    align-items:flex-start;
    justify-content:center;
    padding:32px;
    gap:20px;
    flex-wrap:wrap;
  }

  .video-card{
    width:320px;
    background:var(--card-bg);
    border-radius:12px;
    box-shadow:0 6px 18px rgba(2,6,23,0.5);
    overflow:hidden;
    position:relative;
  }

  .video-wrap{
    position:relative;
    background:#000;
  }

  video{
    display:block;
    width:100%;
    height:180px;
    object-fit:cover;
    background:#000;
  }

  /* Overlay icons (heart, comment, download) */
  .controls {
    position:absolute;
    right:10px;
    top:10px;
    display:flex;
    flex-direction:column;
    gap:8px;
    z-index:10;
  }

  .control-btn{
    width:44px;
    height:44px;
    border-radius:10px;
    display:flex;
    align-items:center;
    justify-content:center;
    background:var(--glass);
    backdrop-filter: blur(4px) saturate(120%);
    cursor:pointer;
    border:1px solid rgba(0,0,0,0.06);
    transition:transform .12s ease, background .12s ease;
  }
  .control-btn:hover{ transform:translateY(-3px); }

  .control-btn img{ width:22px; height:22px; pointer-events:none; }

  /* Heart count */
  .like-count{
    margin-top:6px;
    font-weight:700;
    text-align:center;
    color:var(--muted);
    font-size:13px;
  }

  .card-body{
    padding:12px;
  }
  .title{ font-size:15px; margin:0 0 8px 0; color:#111; }
  .meta{ color:var(--muted); font-size:13px; margin-bottom:8px; }

  /* Comments area */
  .comments{
    border-top:1px solid #efefef;
    padding:10px;
    background:linear-gradient(180deg, rgba(0,0,0,0.02), transparent);
  }
  .comment-list{ max-height:110px; overflow:auto; margin-bottom:8px; font-size:13px; }
  .comment{ padding:6px 8px; border-radius:8px; background:#f6f6f8; margin-bottom:6px; }
  .comment-form{ display:flex; gap:8px; }
  .comment-form input{
    flex:1; padding:8px 10px; border-radius:8px; border:1px solid #ddd; font-size:13px;
  }
  .comment-form button{
    padding:8px 12px; border-radius:8px; border:none; background:var(--accent); color:#fff; cursor:pointer;
  }

  /* small helper */
  .hidden{ display:none; }

  /* Heart active style */
  .liked{ background: linear-gradient(180deg,#ffd1dd,#ff7aa3); box-shadow:0 6px 18px rgba(255,71,111,0.18); }
  .liked img{ filter: drop-shadow(0 1px 0 rgba(0,0,0,0.12)); }

  /* Responsive */
  @media (max-width:740px){
    body{ padding:16px; justify-content:center; }
    .video-card{ width:100%; max-width:420px; }
  }
<!DOCTYPE html><html lang="fr">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Barre de recherche</title>
<style>
  body {
    font-family: Arial, sans-serif;
    display: flex;
    justify-content: center;
    padding-top: 50px;
    background: #f1f1f1;
  }.search-container {
width: 300px;
position: relative;
}

input[type="text"] {
width: 100%;
padding: 12px 20px;
border-radius: 24px;
border: 1px solid #ccc;
outline: none;
font-size: 16px;
box-shadow: 0 2px 5px rgba(0,0,0,0.1);
transition: all 0.2s ease;
}

input[type="text"]:focus {
border-color: #4285f4;
box-shadow: 0 4px 12px rgba(66,133,244,0.3);
}

.search-btn {
position: absolute;
right: 10px;
top: 50%;
transform: translateY(-50%);
border: none;
background: #4285f4;
color: white;
padding: 8px 12px;
border-radius: 50%;
cursor: pointer;
font-size: 16px;
}

.search-btn:hover {
background: #3367d6;
}
</style>

</head>
<body><div class="search-container">
  <input type="text" id="search" placeholder="Rechercher...">
  <button class="search-btn" onclick="search()">ðŸ”</button>
</div><script>
  function search() {
    const query = document.getElementById('search').value.trim();
    if(query) {
      // Exemple simple : ouvrir une recherche Google dans un nouvel onglet
      const url = `https://www.google.com/search?q=${encodeURIComponent(query)}`;
      window.open(url, '_blank');
    }
  }

  // Permet de rechercher avec la touche "EntrÃ©e"
  document.getElementById('search').addEventListener('keypress', function(e){
    if(e.key === 'Enter') search();
  });
</script></body>
</html>
		</style>
	</head>
	<marquee><h1><i>actualites</i></h1></marquee>
	<link rel="stylesheet" href="kyrr.css"/>
	<body>

  <!-- Example video card (x3) -->
  <div class="video-card" data-id="1">
    <div class="video-wrap">
      <video src="tik dengue officiel.mp4" preload="metadata" playsinline></video>
      <div class="controls" aria-hidden="false">
        <div class="control-btn btn-like" title="Like" role="button" aria-pressed="false">
          <img src="data:image/svg+xml;utf8,<svg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 24 24' fill='%23FF476F'><path d='M12 21s-7-4.5-9.2-7.3C-0.6 10.2 2 6 6.1 6c2.1 0 3.6 1.2 4 2 .4-.8 1.9-2 4-2 4.1 0 6.7 4.2 3.3 7.7C19 16.5 12 21 12 21z'/></svg>" alt="coeur" />
        </div>
        <div class="control-btn btn-comment" title="Commenter" role="button">
          <img src="data:image/svg+xml;utf8,<svg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 24 24' fill='%23000'><path d='M2 2v16l4-4h12V2z'/></svg>" alt="comment" />
        </div>
        <div class="control-btn btn-download" title="TÃ©lÃ©charger" role="button">
          <img src="data:image/svg+xml;utf8,<svg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 24 24' fill='%23000'><path d='M5 20h14v-2H5v2zm7-18L5.33 9h3.34v4h4.66V9h3.34L12 2z'/></svg>" alt="download" />
        </div>
      </div>
    </div>

    <div class="card-body">
      <h3 class="title">tik dengue officiel</h3>
      <div class="meta">Auteur Â· 1.2k vues</div>
      <div style="display:flex;gap:12px;align-items:center">
        <div class="like-count" aria-live="polite">0</div>
        <div style="font-size:13px;color:var(--muted)">Likes</div>
      </div>
    </div>

    <div class="comments hidden" aria-hidden="true">
      <div class="comment-list"></div>

      <div class="comment-form">
        <input type="text" class="comment-input" placeholder="Ã‰crire un commentaire..." aria-label="Ã‰crire un commentaire">
        <button class="btn-post">Envoyer</button>
      </div>
    </div>
  </div>

  <!-- Duplique la carte (change data-id) si tu veux plus de vidÃ©os -->
  <div class="video-card" data-id="2">
    <div class="video-wrap">
      <video src="Franglish_-_Djo_ft._Aya_Nakamura_et_Hamza_(Audio_Officiel)(144p).mp4" preload="metadata" playsinline></video>
      <div class="controls">
        <div class="control-btn btn-like" title="Like" role="button" aria-pressed="false">
          <img src="data:image/svg+xml;utf8,<svg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 24 24' fill='%23FF476F'><path d='M12 21s-7-4.5-9.2-7.3C-0.6 10.2 2 6 6.1 6c2.1 0 3.6 1.2 4 2 .4-.8 1.9-2 4-2 4.1 0 6.7 4.2 3.3 7.7C19 16.5 12 21 12 21z'/></svg>" alt="coeur" />
        </div>
        <div class="control-btn btn-comment" title="Commenter" role="button">
          <img src="data:image/svg+xml;utf8,<svg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 24 24' fill='%23000'><path d='M2 2v16l4-4h12V2z'/></svg>" alt="comment" />
        </div>
        <div class="control-btn btn-download" title="TÃ©lÃ©charger" role="button">
          <img src="data:image/svg+xml;utf8,<svg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 24 24' fill='%23000'><path d='M5 20h14v-2H5v2zm7-18L5.33 9h3.34v4h4.66V9h3.34L12 2z'/></svg>" alt="download" />
        </div>
      </div>
    </div>

    <div class="card-body">
      <h3 class="title">Franglish_-_Djo_ft._Aya_Nakamura_et_Hamza</h3>
      <div class="meta">Auteur Â· 450 vues</div>
      <div style="display:flex;gap:12px;align-items:center">
        <div class="like-count">0</div>
        <div style="font-size:13px;color:var(--muted)">Likes</div>
      </div>
    </div>

    <div class="comments hidden" aria-hidden="true">
      <div class="comment-list"></div>
      <div class="comment-form">
        <input type="text" class="comment-input" placeholder="Ã‰crire un commentaire..." aria-label="Ã‰crire un commentaire">
        <button class="btn-post">Envoyer</button>
      </div>
    </div>
  </div>

  <div class="video-card" data-id="3">
    <div class="video-wrap">
      <video src="mv_storyop_pakchunk1.mp4" preload="metadata" playsinline></video>
      <div class="controls">
        <div class="control-btn btn-like" title="Like" role="button" aria-pressed="false">
          <img src="data:image/svg+xml;utf8,<svg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 24 24' fill='%23FF476F'><path d='M12 21s-7-4.5-9.2-7.3C-0.6 10.2 2 6 6.1 6c2.1 0 3.6 1.2 4 2 .4-.8 1.9-2 4-2 4.1 0 6.7 4.2 3.3 7.7C19 16.5 12 21 12 21z'/></svg>" alt="coeur" />
        </div>
        <div class="control-btn btn-comment" title="Commenter" role="button">
          <img src="data:image/svg+xml;utf8,<svg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 24 24' fill='%23000'><path d='M2 2v16l4-4h12V2z'/></svg>" alt="comment" />
        </div>
        <div class="control-btn btn-download" title="TÃ©lÃ©charger" role="button">
          <img src="data:image/svg+xml;utf8,<svg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 24 24' fill='%23000'><path d='M5 20h14v-2H5v2zm7-18L5.33 9h3.34v4h4.66V9h3.34L12 2z'/></svg>" alt="download" />
        </div>
      </div>
    </div>

    <div class="card-body">
      <h3 class="title">video de dragon ball Z</h3>
      <div class="meta">Auteur Â· 2.1k vues</div>
      <div style="display:flex;gap:12px;align-items:center">
        <div class="like-count">0</div>
        <div style="font-size:13px;color:var(--muted)">Likes</div>
      </div>
    </div>

    <div class="comments hidden" aria-hidden="true">
      <div class="comment-list"></div>
      <div class="comment-form">
        <input type="text" class="comment-input" placeholder="Ã‰crire un commentaire..." aria-label="Ã‰crire un commentaire">
        <button class="btn-post">Envoyer</button>
      </div>
    </div>
  </div>

<script>
/*
  Comportement :
  - Like: toggle like/unlike, mettre Ã  jour compteur et apparence
  - Comment: montre/cachÐµ la zone de commentaire, publier affiche le commentaire
  - Download: essaie de rÃ©cupÃ©rer la vidÃ©o puis force le tÃ©lÃ©chargement (fallback: <a download>)
*/
document.addEventListener('DOMContentLoaded', () => {
  const cards = document.querySelectorAll('.video-card');

  cards.forEach(card => {
    const likeBtn = card.querySelector('.btn-like');
    const commentBtn = card.querySelector('.btn-comment');
    const dlBtn = card.querySelector('.btn-download');
    const likeCountEl = card.querySelector('.like-count');
    const commentsWrap = card.querySelector('.comments');
    const commentList = card.querySelector('.comment-list');
    const commentInput = card.querySelector('.comment-input');
    const postBtn = card.querySelector('.btn-post');
    const video = card.querySelector('video');

    // store state (basic, in-memory)
    let state = { liked: false, likes: 0, comments: [] };

    // Like button handler
    likeBtn.addEventListener('click', () => {
      state.liked = !state.liked;
      state.likes += state.liked ? 1 : -1;
      if (state.likes < 0) state.likes = 0;
      updateLikeUI();
    });

    function updateLikeUI(){
      likeCountEl.textContent = state.likes;
      likeBtn.setAttribute('aria-pressed', String(state.liked));
      if(state.liked) likeBtn.classList.add('liked');
      else likeBtn.classList.remove('liked');
    }

    // Comment toggle
    commentBtn.addEventListener('click', () => {
      const isHidden = commentsWrap.classList.contains('hidden');
      commentsWrap.classList.toggle('hidden');
      commentsWrap.setAttribute('aria-hidden', String(!isHidden));
      if (!isHidden) commentInput.blur();
      else commentInput.focus();
    });

    // Post comment
    postBtn.addEventListener('click', postComment);
    commentInput.addEventListener('keydown', (e) => {
      if (e.key === 'Enter') postComment();
    });

    function postComment(){
      const text = commentInput.value.trim();
      if (!text) return;
      state.comments.unshift({ text, at: new Date().toLocaleString() });
      renderComments();
      commentInput.value = '';
    }

    function renderComments(){
      commentList.innerHTML = '';
      if (state.comments.length === 0) {
        commentList.innerHTML = '<div style="color:#888;font-size:13px">Aucun commentaire â€” sois le premier !</div>';
        return;
      }
      for (const c of state.comments) {
        const div = document.createElement('div');
        div.className = 'comment';
        div.innerHTML = `<strong style="font-size:13px">Utilisateur</strong> <span style="color:#999;font-size:11px;margin-left:6px">${c.at}</span><div style="margin-top:6px;font-size:13px">${escapeHtml(c.text)}</div>`;
        commentList.appendChild(div);
      }
    }

    // Download handler
    dlBtn.addEventListener('click', async () => {
      const src = video.currentSrc || video.src;
      if (!src) return alert('Source vidÃ©o introuvable.');
      // Try to fetch blob (works if CORS allows)
      try {
        const res = await fetch(src, { mode: 'cors' });
        if (!res.ok) throw new Error('Ã‰chec du tÃ©lÃ©chargement');
        const blob = await res.blob();
        const url = URL.createObjectURL(blob);
        triggerDownload(url, filenameFromUrl(src));
        // revoke after a bit
        setTimeout(()=>URL.revokeObjectURL(url), 30000);
      } catch (err) {
        // Fallback : use direct link with download attribute (may fail cross-origin)
        triggerDownload(src, filenameFromUrl(src));
      }
    });

    function triggerDownload(href, name){
      const a = document.createElement('a');
      a.href = href;
      a.download = name || 'video.mp4';
      document.body.appendChild(a);
      a.click();
      setTimeout(()=>a.remove(), 50);
    }

    function filenameFromUrl(url){
      try {
        const u = new URL(url);
        const p = u.pathname.split('/').pop();
        return p || 'video.mp4';
      } catch(e){
        return 'video.mp4';
      }
    }

    function escapeHtml(s){
      return s.replace(/[&<>"']/g, ch => ({'&':'&amp;','<':'&lt;','>':'&gt;','"':'&quot;',"'":'&#39;'}[ch]));
    }

    // initial render
    updateLikeUI();
    renderComments();
  });
});
</script>
</body>
</html>
