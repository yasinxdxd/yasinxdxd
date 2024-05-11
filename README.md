<style>
.all {
    background-color: rgb(32, 37, 43);
}
* {
    background-color: rgb(32, 37, 43);
}

.wrapper {
    height: 100vh;
    /*This part is important for centering*/
    display: grid;
    place-items: center;
}

.typing-demo {
    width: 26ch;
    animation: typing 2s steps(26), blink .5s step-end infinite alternate;
    white-space: nowrap;
    overflow: hidden;
    border-right: 3px solid bisque;
    font-family: monospace;
    font-size: 3em;
    letter-spacing: 0px;
    word-spacing: 0px;
}

.func {
    color:blueviolet;
    animation: glow-pink 1s ease-in-out infinite alternate;
}
.text {
    color:darkcyan;
    animation: glow-green 1s ease-in-out infinite alternate;
}
.paran {
    color:bisque;
}

@keyframes typing {
    from {
        width: 0
    }
}
    
@keyframes blink {
    0% {
        border-color: bisque;
    }
    40% {
        border-color: bisque;
    }
    60% {
        border-color: transparent;
    }
    80% {
        border-color: bisque;
    }
}

@keyframes glow-pink {
    from {
        text-shadow: 0 0 2px #fff, 0 0 2px rgb(157, 73, 235), 0 0 2px rgb(157, 73, 235), 0 0 2px rgb(157, 73, 235), 0 0 2px rgb(157, 73, 235), 0 0 6px rgb(157, 73, 235), 0 0 7px rgb(157, 73, 235);
        
    }
    to {
        text-shadow: 0 0 0px #fff, 0 0 0px #fff, 0 0 0px blueviolet, 0 0 0px blueviolet, 0 0 3px blueviolet, 0 0 0px blueviolet, 0 0 0px blueviolet;
    }
}

@keyframes glow-green {
    from {
        text-shadow: 0 0 0px #fff, 0 0 0px #fff, 0 0 0px darkcyan, 0 0 0px darkcyan, 0 0 0px darkcyan, 0 0 0px darkcyan, 0 0 0px darkcyan;
    }
    to {
        text-shadow: 0 0 2px #fff, 0 0 2px rgb(23, 150, 150), 0 0 2px rgb(23, 150, 150), 0 0 2px rgb(23, 150, 150), 0 0 2px rgb(23, 150, 150), 0 0 6px rgb(23, 150, 150), 0 0 7px rgb(23, 150, 150);
    }
}
</style>

<div class="all">
    <div class="wrapper">
        <div class="typing-demo">
            <span class="func">print</span>
            <span class="paran">(</span>
            <span class="text">"Hello, World!"</span>
            <span class="paran">)</span>
        </div>
    </div>
</div>
