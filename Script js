document.getElementById('videoForm').addEventListener('submit', function(event) {
    event.preventDefault();
    
    const videoUrl = document.getElementById('videoUrl').value;
    
    if (videoUrl) {
        // Cria um elemento de vídeo e adiciona ao DOM
        const videoElement = document.createElement('div');
        videoElement.classList.add('video');
        
        const iframe = document.createElement('iframe');
        iframe.src = videoUrl;
        iframe.width = 320;
        iframe.height = 240;
        iframe.frameborder = "0";
        iframe.allow = "accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture";
        iframe.allowfullscreen = true;
        
        videoElement.appendChild(iframe);
        document.getElementById('videoList').appendChild(videoElement);
        
        // Limpar campo após adicionar
        document.getElementById('videoUrl').value = '';
    }
});
