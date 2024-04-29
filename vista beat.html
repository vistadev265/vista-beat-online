<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Vista Beat</title>
    <style>
        /* Define styles here if needed */
    </style>
</head>
<body>
    <canvas id="gameCanvas" width="800" height="600"></canvas>
    <script>
        // Initialize canvas and context
        var canvas = document.getElementById("gameCanvas");
        var ctx = canvas.getContext("2d");

        // Colors
        var WHITE = "#FFFFFF";
        var RED = "#FF0000";
        var BLUE = "#0000FF";

        // Fonts
        var fontLarge = "48px Arial";
        var fontMedium = "36px Arial";
        var fontSmall = "24px Arial";

        // Game variables
        var score = 0;
        var cubes = [];
        var cubeSpeed = 8;
        var cubeSpawnFrequency = 999;

        // Function to generate a new cube
        function generateCube() {
            var size = Math.floor(Math.random() * (50 - 20 + 1)) + 20;
            var x = Math.floor(Math.random() * (canvas.width - size));
            var y = -size;
            var color = (Math.random() < 0.5) ? RED : BLUE;
            cubes.push({x: x, y: y, size: size, color: color});
        }

        // Function to draw text on screen
        function drawText(text, font, color, x, y) {
            ctx.font = font;
            ctx.fillStyle = color;
            ctx.fillText(text, x, y);
        }

        // Main game loop
        function gameLoop() {
            // Clear the canvas
            ctx.clearRect(0, 0, canvas.width, canvas.height);

            // Update game state
            // Spawn new cubes
            generateCube();

            // Move cubes
            for (var i = 0; i < cubes.length; i++) {
                cubes[i].y += cubeSpeed;
            }

            // Remove cubes that have passed the bottom of the screen
            cubes = cubes.filter(function(cube) {
                return cube.y < canvas.height;
            });

            // Draw objects
            for (var i = 0; i < cubes.length; i++) {
                ctx.fillStyle = cubes[i].color;
                ctx.fillRect(cubes[i].x, cubes[i].y, cubes[i].size, cubes[i].size);
            }

            // Draw score
            drawText("Score: " + score, fontSmall, WHITE, 10, 30);

            // Call gameLoop recursively
            requestAnimationFrame(gameLoop);
        }

        // Start the game loop
        gameLoop();

        // Event listener for mouse clicks
        canvas.addEventListener("mousedown", function(event) {
            var mouse_x = event.clientX - canvas.getBoundingClientRect().left;
            var mouse_y = event.clientY - canvas.getBoundingClientRect().top;

            for (var i = cubes.length - 1; i >= 0; i--) {
                var cube = cubes[i];
                if (mouse_x >= cube.x && mouse_x <= cube.x + cube.size &&
                    mouse_y >= cube.y && mouse_y <= cube.y + cube.size) {
                    if ((event.which === 1 && cube.color === RED) || 
                        (event.which === 3 && cube.color === BLUE)) {
                        cubes.splice(i, 1);
                        score++;
                    }
                }
            }
        });
    </script>
</body>
</html>
