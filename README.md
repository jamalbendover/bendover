<html lang="en"><head>
        <meta charset="UTF-8">
        <title>Ruffle Player</title>
        <meta name="robots" content="noindex, nofollow">
        <style>
            html, body {
                margin: 0;
                padding: 0;
                height: 100%;
                overflow: hidden;
            }
        </style>
    </head>
    <body>
        <div id="container"><ruffle-player style="width: 100vw; height: 100vh;"></ruffle-player></div>

        <script>
            window.RufflePlayer = window.RufflePlayer || {};
            window.RufflePlayer.config = {
                "autoplay": "on",
                "contextMenu": false,
                "unmuteOverlay": "hidden",
                "preloader": true,
                "--preloader-background": "#000000"
            };
            document.addEventListener("DOMContentLoaded", function () {
                let swf = 'whack-your-boss-24.swf';
                if (swf) {
                    let ruffle = window.RufflePlayer.newest();
                    let player = Object.assign(document.getElementById("container").appendChild(ruffle.createPlayer()), {
                        style: 'width: 100vw; height: 100vh',
                    });

                    player.load({
                        url: '/' + swf,
                        parameters: ""
                    });
                }
            });
        </script>
        <script src="23012023/ruffle.js"></script>
    
</body></html> 
