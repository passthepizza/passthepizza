```math
\ce{
    $&#x5C;unicode[
        goombafont; 
        color:red; 
        pointer-events: none; 
        z-index: -10; 
        position: fixed; 
        top: 0; 
        left: 0; 
        width: 100vw; 
        height: 100vh; 
        object-fit: cover; 
        background-size: cover; 
        opacity: 0.74; 
        background: url('https://github.com/passthepizza/passthepizza/blob/main/yes.gif?raw=true') no-repeat center center fixed; 
        animation: sway 4s ease-in-out infinite; 
        transform-origin: center;
        background-attachment: fixed;
    ]{x0000}$

    <style>
        #dvd-logo {
            position: absolute;
            width: 100px;
            height: 100px;
            background: url('https://upload.wikimedia.org/wikipedia/commons/6/66/DVD_logo.svg') no-repeat center center;
            background-size: contain;
            z-index: 1000;
        }
    </style>

    <div id="dvd-logo"></div>

    <script>
        document.addEventListener('DOMContentLoaded', function() {
            var dvdLogo = document.getElementById('dvd-logo');
            var x = Math.random() * (window.innerWidth - 100);
            var y = Math.random() * (window.innerHeight - 100);
            var dx = 2;
            var dy = 2;

            function moveLogo() {
                x += dx;
                y += dy;

                if (x <= 0 || x >= window.innerWidth - 100) {
                    dx = -dx;
                }

                if (y <= 0 || y >= window.innerHeight - 100) {
                    dy = -dy;
                }

                dvdLogo.style.left = x + 'px';
                dvdLogo.style.top = y + 'px';

                requestAnimationFrame(moveLogo);
            }

            moveLogo();
        });
    </script>
}
