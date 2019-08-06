# pitunweb
pitunweb
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>Wellcome my website</title>
    <link rel="stylesheet" href="css/style.css">
    <link rel="stylesheet" href="css/bootstrap.min.css">
</head>

<body>
    <header>
        <div class="container">
            <div class="row">
                <!-- Logo
                <a href="#" class="logo"><img src="images/pitun.png"></a> -->
                <!-- Menu -->
                <nav id="home-nav">
                    <ul class="main-menu">
                        <li><a href="#">Trang chủ</a></li>
                        <li><a href="#">Giới thiệu</a></li>
                        <li><a href="#">Địa chỉ</a></li>
                        <li><a href="#">Liên hệ</a></li>
                    </ul>
                    <div class="menu-trigger">
                        <span class="span-1"></span>
                        <span class="span-2"></span>
                        <span class="span-3"></span>
                    </div>
                </nav>
                <!-- search -->
                <div class="search-box">
                    <form>
                        <input class="sb-text" type="text" placeholder="tim kiem">
                        <input class="sb-sbm" type="submit">
                    </form>
                </div>
            </div>
            <div class="menu-container">
                <div class="container">
                    <ul id="menu" class="clearfix">
                        <li>
                            <a href="#">1</a>
                            <ul class="sub-menu">
                                <li><a href="#"></a>1.1</li>
                                <li><a href="#"></a>1.2</li>
                                <li><a href="#"></a>1.3</li>
                            </ul>
                        </li>
                        <li><a href="#">2</a></li>
                        <li><a href="#">3</a></li>
                        <li><a href="#">4</a></li>
                        <li><a href="#">5</a></li>
                    </ul>
                </div>
            </div>
        </div>
    </header>

    <section id="hero-image">
        <div class="hero-content text-center">
            <h1 class="title">PiTun Blog</h1>
            <p class="sub-title">Wellcome</p>
        </div>
        <a class="btn-xn" href="#gioi-thieu">Xem Ngay</a>
    </section>
    <section id="gioi-thieu" class="section-padding">
        <div class="container text-center">
            <h2 class="title">Giới thiệu về bản thân</h2>
            <p class="sub-title"> - Nguyễn Đoàn Liên Sơn - </p>
            <div class="row">
                <div class="col-lg-4">
                    <div class="item">
                        <figure>
                            <img src="images/thongtinchitiet.png" alt="">
                            <figcaption>
                                <h3>Xin chào các bạn đã ghé thăm</h3>
                                <p>Đây là một số thông tin chi tiết về mình.</p>
                                <a class="btn-xn" href="#">Xem Thêm</a>
                            </figcaption>
                        </figure>
                    </div>
                </div>
                <div class="col-lg-4">
                    <div class="item">
                        <figure>
                            <img src="images/kynang.png" alt="">
                            <figcaption>
                                <h3>Xin chào các bạn đã ghé thăm</h3>
                                <p>Đây là một số kỹ năng nổi bật nhất của mình</p>
                                <a class="btn-xn" href="#">Xem Thêm</a>
                            </figcaption>
                        </figure>
                    </div>
                </div>
                <div class="col-lg-4">
                    <div class="item">
                        <figure>
                            <img src="images/sothich.png" alt="">
                            <figcaption>
                                <h3>Xin chào các bạn đã ghé thăm</h3>
                                <p>Cùng khám phá sở thích của mình nhé!</p>
                                <a class="btn-xn" href="#">Xem Thêm</a>
                            </figcaption>
                        </figure>
                    </div>
                </div>
            </div>
        </div>
    </section>
    <section id="gioi-thieu2" class="section-padding">
        <div class="container text-center">
            <h2 class="title">hello word</h2>
            <p class="sub-title">IamPiTun</p>
        </div>
    </section>


    <script src="js/jquery-3.3.1.js"></script>
    <script>
        $(document).ready(function () {

            //Menu
            $(".menu-trigger").click(function () {
                $(".menu-container").toggleClass("open");
                $(".menu-trigger span").toggleClass("open");
            });

            //search
            $(".sb-sbm").click(function (event) {
                if ($(".sb-text").val().length <= 0) {
                    event.preventDefault();
                }

                $(".sb-text").toggleClass("open");
            });
        });
    </script>
</body>

</html>
