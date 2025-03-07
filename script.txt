window.onload = function() {
    setTimeout(() => {
        document.getElementById('popup').style.display = 'block';
    }, 3000); // 3-second delay

    var audio = document.getElementById("background-music");
    audio.play().catch(error => {
        console.log("Autoplay blocked. User interaction required.");
    });
};
