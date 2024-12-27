section {
    display: flex;
    flex-wrap: wrap;
}
.container1 {
    display: flex;
    flex-wrap: wrap;
    width: 600px;
    height: 500px;
    padding: 75px 90px;
    margin-left: 120px;
}
.headings {
    text-align: center;
    text-decoration: underline;
    text-underline-offset: 10px;
    text-decoration-thickness: 5px;
    margin-bottom: 50px;
}
.bar {
    font-size: 23px;

}

.Technical-bars .bar {
    margin-top: 40px 0;

}

.Technical-bars .bar:first-child {
    margin-top: 0;
}

.Technical-bars .bar:last-child {
    margin-bottom: 0;
}

.Technical-bars .bar .info {
    margin-bottom: 5px;
}

.Technical-bars .bar .info span {
    font-size: 17px;
    font-weight: 500;
    animation: showText 0, 5s linear forwards;
    opacity: 0;
}

.Technical-bars .bar .progress-line {
    position: relative;
    border-radius: 10px;
    width: 100%;
    height: 5px;
    background-color: #ffffff;
    animation: animate 1s cubic-bezier(1, 0, 0, 5, 1) forwards;
    transform: scaleX(0);
    transform-origin: left;
}

@keyframes animate {
    100% {
        transform: scaleX(1);
        transform: o;
    }
}

.Technical-bars .bar .progress-line span {
    height: 100%;
    background-color: #ff004f;
    position: absolute;
    border-radius: 10px;
    animation: animate 1s cubic-bezier(1, 0, 0, 5, 1) forwards;
    transform: scaleX(0);
    transform-origin: left;

}

.progress-line .java span {
    width: 80%;
}

.progress-line .html span {
    width: 90%;
}

.progress-line .css span {
    width: 60%;
}

.progress-line .js span {
    width: 59%;
}

.progress-line .bootstrap span {
    width: 80%;
}

.progress-line .oracle span {
    width: 70%;
}

.progress-line .sql span {
    width: 75%;
}

.progress-line span::after {
    position: absolute;
    padding: 1px 8px;
    background-color: #262626;
    color: #fff;
    font-size: 12px;
    border-radius: 3px;
    top: -28px;
    animation: showText 0.5s 1.5s linear forwards;
    opacity: 0;
}

.progress-line .java span::after {
    content: "80%";
}

.progress-line .html span::after {
    content: "90%";
}

.progress-line .css span::after {
    content: "80%";
}

.progress-line .js span::after {
    content: "59%";
}

.progress-line .bootstrap span::after {
    content: "80%";
}

.progress-line .oracle span::after {
    content: "70%";
}

.progress-line .sql span::after {
    content: "75%";
}

.progress-line span::before {
    content: "";
    position: absolute;
    width: 0;
    height: 0;
    border: 7px solid transparent;
    border-bottom-width: 0px;
    border-right-width: 0px;
    border-top-color: #262626;
    top: -10px;
    right: 0;
    animation: showText 0.5s 1.5s linear forwards;
    opacity: 0;

}

@keyframes showText {
    100% {
        opacity: 1;
    }
}

.radial-bars {
    width: 100%;
    display: flex;
    flex-wrap: wrap;
    justify-content: space-evenly;
    align-items: flex-start;
}

.radial-bars .radial-bar {
    width: 50%;
    height: 170px;
    margin-bottom: 10px;
    position: relative;

}

.radial-bars .radial-bar svg {
    position: absolute;
    top: 50%;
    transform: translate(-50%, -50%) rotate(-90deg);
    width: 120px;
    height: 160px;
}

.radial-bars .radial-bar .progress-bar {
    stroke-width: 10;
    stop-color: #262626;
    fill: transparent;
    stroke-dasharray: 502;
    stroke-dashoffset: 502;
    stroke-linecap: round;
    animation: animate-bar 1s linear forwards;

}

@keyframes animate-bar {
    100% {
        stroke-dashoffset: -1;
    }
}

.path {
    stroke-width: 10;
    stroke: #ff004f;
    fill: transparent;
    stroke-dasharray: 502;
    stroke-dashoffset: 502;
    stroke-linecap: round;
}

.path-1 {
    animation: animate-path1 1s 1s linear forwards;
}

.path-2 {
    animation: animate-path2 1s 1s linear forwards;
}

.path-3 {
    animation: animate-path3 1s 1s linear forwards;
}

.path-4 {
    animation: animate-path4 1s 1s linear forwards;
}

@keyframes animate-path1 {
    100% {
        stroke-dashoffset: 50;
    }
}

@keyframes animate-path2 {
    100% {
        stroke-dashoffset: 175;
    }
}

@keyframes animate-path3 {
    100% {
        stroke-dashoffset: 125;
    }
}

@keyframes animate-path4 {
    100% {
        stroke-dashoffset: 75;
    }
}

.radial-bar .percentage {

    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    font-size: 17px;
    font-weight: 500;
    animation: showText 0.5s 1s linear forwards;
    opacity: 0;
}

.redial-bar .skilltext {
    width: 100%;
    position: absolute;
    text-align: center;
    left: 50%;
    bottom: -5px;
    transform: translateX(-50px);
    font-size: 17px;
    font-weight: 500;
    animation: showText 0.5s 1s linear forwards;
    opacity: 0;
}
<h1 class="Sub-Title">My Skills</h1>
    <section>
        <div id="Skills" class="container1">
            <h1 class="headings">Technical Skills</h1>
            <div class="Technical-bars">
                <div class="bar"><i style="color: #ff0000;" class="fa-brands fa-java"></i>
                    <div class="info">
                        <span>Java</span>
                    </div>
                    <div class="progress-line java">
                        <span></span>
                    </div>
                </div>
                <div class="bar"><i style="color: #c95d2e;" class="fa-brands fa-html5"></i>
                    <div class="info">
                        <span>HTML</span>
                    </div>
                    <div class="progress-line html">
                        <span></span>
                    </div>
                </div>
                <div class="bar"><i style="color: #147bbc;" class="fa-brands fa-css3-alt"></i>
                    <div class="info">
                        <span>CSS</span>
                    </div>
                    <div class="progress-line css">
                        <span></span>
                    </div>
                </div>
                <div class="bar"><i style="color: #b0bc1e;" class="fa-brands fa-js"></i>
                    <div class="info">
                        <span>JavaScript</span>
                    </div>
                    <div class="progress-line js">
                        <span></span>
                    </div>
                </div>
                <div class="bar"><i style="color: #b0bc;" class="fa-brands fa-bootstrap"></i>
                    <div class="info">
                        <span>BootStrap</span>
                    </div>
                    <div class="progress-line bootstrap">
                        <span></span>
                    </div>
                </div>
                <div class="bar"><i style="color: #ff6200;" class="fa-solid fa-database"></i>
                    <div class="info">
                        <span>Oracle</span>
                    </div>
                    <div class="progress-line oracle">
                        <span></span>
                    </div>
                </div>
                <div class="bar"><i style="color: #2000b0;" class="fa-solid fa-database"></i>
                    <div class="info">
                        <span>SQL</span>
                    </div>
                    <div class="progress-line sql">
                        <span></span>
                    </div>
                </div>
            </div>
        </div>
        <div class="container1">
            <h2 class="headings">Professional Skills</h2>
            <div class="radial-bars">
                <svg x="0px" y="0px" viewBox="0 0 200 200">
                    <circle class="progress-bar" cx="100" cy="100" r="80"></circle>
                    <circle class="path path-1" cx="100" cy="100" r="80"></circle>

                </svg>
                <div class="percentage">90%</div>
                <div class="skilltext">Creativity</div>
            </div>
            <div class="radial-bars">
                <svg x="0px" y="0px" viewBox="0 0 200 200">
                    <circle class="progress-bar" cx="100" cy="100" r="80"></circle>
                    <circle class="path path-2" cx="100" cy="100" r="80"></circle>

                </svg>
                <div class="percentage">70%</div>
                <div class="skilltext">Communication</div>
            </div>
            <div class="radial-bars">
                <svg x="0px" y="0px" viewBox="0 0 200 200">
                    <circle class="progress-bar" cx="100" cy="100" r="80"></circle>
                    <circle class="path path-3" cx="100" cy="100" r="80"></circle>

                </svg>
                <div class="percentage">75%</div>
                <div class="skilltext">Problem Solving</div>
            </div>
            <div class="radial-bars">
                <svg x="0px" y="0px" viewBox="0 0 200 200">
                    <circle class="progress-bar" cx="100" cy="100" r="80"></circle>
                    <circle class="path path-4" cx="100" cy="100" r="80"></circle>

                </svg>
                <div class="percentage">85%</div>
                <div class="skilltext">Team-Work</div>
            </div>
        </div>
    </section>

        <!-- --------------------portfolio------------------- -->

        <div id="portfolio">
            <div class="container">
                <h1 class="Sub-Title">My Work</h1>
                <div class="worklist">
                    <div class="work">
                        <img src="/public/images/work1.png" alt="">
                        <div class="layer">
                            <h3>Online Bank Management System</h3>
                            <p>The Online Banking Management System utilizes Java Swing for frontend, ensuring a
                                user-friendly
                                interface, and MySQL for backend, ensuring secure data management. </p>
                            <a href="#"><i class="fa-sharp fa-solid fa-arrow-up-right-from-square"></i></a>

                        </div>
                    </div>
                    <div class="work">
                        <img src="/public/images/work2.png" alt="">
                        <div class="layer">
                            <h3>Online Result Management System</h3>
                            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Voluptates explicabo
                                consequuntur tenetur vero nam doloribus.</p>
                            <a href="#"><i class="fa-sharp fa-solid fa-arrow-up-right-from-square"></i></a>
                        </div>
                    </div>

                    <div class="work">
                        <img src="/public/images/work3.jpg" alt="">
                        <div class="layer">
                            <h3>Interior Desigining eCommerce Web</h3>
                            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Voluptates explicabo
                                consequuntur tenetur vero nam doloribus.</p>
                            <a href="#"><i class="fa-sharp fa-solid fa-arrow-up-right-from-square"></i></a>
                        </div>
                    </div>
                </div>
                <a href="#" class="btn">See More</a>
            </div>
        </div>