<script>
    import { Swipe, SwipeItem } from "svelte-swipe";

    const swipeConfig = {
    autoplay: false,
    delay: 2000,
    showIndicators: false,
    transitionDuration: 1000,
    defaultIndex: 0,
    };
    let SwipeComp;

    function nextSlide(){
    SwipeComp.nextItem()
    }

    function prevSlide(){
        SwipeComp.prevItem()
    }
</script>

<main id="main">
    
    <div class="intro">
        <div class="intro__note">
            <h1>Nền tảng tài chính thông minh hàng đầu trên thế giới</h1>
            <p>Tham gia Bitkingreturns của chúng tôi để xây dựng một nền kinh tế phi tập trung hoàn toàn minh bạch</p>
            <div>
            <button class="btn-join">Tham gia</button>
            <a href="">Tìm hiểu thêm</a>
            <img src="assets/Group.png" alt="">
            </div>
        </div>
        
            <img src="assets/Group40.png" alt="">
        
    </div>
    <div class="titlebar">
        <img src="assets/bcio.png" alt="">
        <img src="assets/Groupdes.png" alt="">
        <img src="assets/galaxy-technology logo.png" alt="">
        <img src="assets/Groupboxster.png" alt="">
        <img src="assets/Techkon_logo logo.png" alt="">
    </div>
    <div class="catagory">
        <h3>Khoản đầu tư tốt nhất cho bạn</h3>
        <div class="inves">
            <div class="invest__catagory">
                <img src="assets/Monopol.png" alt="">
                <h2>Độc quyền</h2>
                <p class="content">Chúng tôi đã tạo ra công thức cho một nền kinh tế tự động thông minh. Nơi mà mỗi cá nhân đều có thể tham gia dễ dàng và tạo ra nhiều lợi nhuận</p>                
            </div>
            <div class="invest__catagory">
                <img src="assets/Easy.png" alt="">
                <h2>Đơn giản</h2>
                <p class="content">Hệ thống trải nghiệm người dùng đơn giản, không yêu cầu KYC, không giới hạn rút và nạp tiền</p>
            </div>
            <div class="invest__catagory">
                <img src="assets/clear.png" alt="">
                <h2>Minh bạch</h2>
                <p>Bạn có thể biết được mọi thứ ở đây. Chúng tôi là một trong những nền tảng đáng tin cậy nhất trên thế giới</p>
            </div>
        </div>
    </div>
    
    <div class="codeSumary">
        <img src="assets/Frame17.png" alt="">
        <div class="code__btr">
            <p>Mua btr</p>
            <h3>Mã thông báo trên TRON tốt nhất</h3>
            <p>Chúng tôi sử dụng TRON như một công nghệ mới và xây dựng BTR trên nền tảng hợp 
                đồng thông minh. TRON giúp cung cấp đầy đủ công cụ để 
                tạo ra những mã thông báo hàng đầu trên thế giới, trong đó bao gồm BTR 
                – hứa hẹn sẽ phát triển mạnh mẽ trong năm 2021</p>
            <button class="code__join">Tham gia
                <img src="assets/code_join.png" alt="">
            </button>
        </div>
    </div>
    
    <div class="benefit">
        <h3>Lợi ích của Bitkingreturns</h3>
        
        <div class="benefit__1">
            <div class="bene">
            
            </div>
            <div class="content">
                <img src="assets/1.png" alt="" class="img_1">
                <h4>Chia sẻ giúp bạn tạo ra một khoản lợi nhuận lớn mỗi ngày</h4>
                <p>Bạn sẽ nhận được nhiều hoa hồng mỗi ngày thông qua số lượng vé mua mà bạn đã giới thiệu. Nền tảng Bitkingreturns hoàn toàn tự động rút tiền và nạp tiền.</p>
                <div class="more"></div>
                <a href="">Read more</a>
                <img src="assets/number.png" alt="">
            </div>
            <img class="img-benefit" src="assets/Asset21.png" alt="">
        </div>
        <div class="benefit__2">
            <div class="bene__2">
                
                </div>
                
            <img class="img-benefit" src="assets/Asset20.png" alt="">
            
            <div class="content ">
                <img src="assets/2.png" alt="" class="img_1">
                <h4>Hệ thống bảo vệ tài sản nhiều tầng</h4>
                <p>Chúng tôi đã xây dựng hệ thống bảo vệ chắc chắn và chi tiết để ngăn chặn những tin tặc, những kẻ lừa đảo tấn công và lấy cắp tài sản của bạn</p>
                <div class="more"></div>
                <a href="">Read more</a>
                <img src="assets/number.png" alt="">
            </div>
        </div>
        <div class="benefit__3">
            <div class="bene__3">
             
            </div>
            <div class="content">
                <img src="assets/3.png" alt="" class="img_1">
                <h4>Kiếm tiền trở nên dễ dàng với Bitkingreturns</h4>
                <p>Bạn đang tìm kiếm một nền tảng tài chính an toàn, đáng tin cậy và tạo ra nhiều lợi nhuận trong tương lai? Vậy thì Bitkingreturns - nền tảng được xây dựng trên công trình nghiên cứu của hơn 30 giáo sư kinh tế hàng đầu trên thế giới - chính là giải pháp hoàn hảo cho bạn.</p>
                <div class="more"></div>
                <a href="">Read more</a>
                <img src="assets/number.png" alt="">
            </div>
            <img class="img-benefit" src="assets/active.png" alt="">
        </div>
        <div class="aa">
            <div class="bene__4">
                
            </div>
        </div>
    </div>
    <div class="slider">
        <div class="slider__tab">
            <div class="tab--swipe">
            <Swipe bind:this={SwipeComp} {...swipeConfig}>
                <SwipeItem>
                    <div class="swipeitem">
                        <div class="swipe__1">
                            <div class="content">
                                <img src="assets/Star.png" alt="">
                                <h3>Mua vé</h3>
                                <p>Mua vé của bạn để bắt đầu đầu tư</p>
                            </div>
                        </div>
                        <div class="swipe__2">
                            <div class="content">
                                <img src="assets/Star.png" alt="">
                                <h3>Theo dõi lợi nhuận</h3>
                                <p>Theo dõi lợi nhuận của từng vé</p>
                            </div>
                        </div>
                        <div class="swipe__3">
                            <div class="content">
                                <img src="assets/Star.png" alt="">
                                <h3>Chia sẻ</h3>
                                <p>Chia sẻ để xây dựng khoản lợi nhuận lớn mỗi ngày</p>
                            </div>
                        </div>
                    </div>
                </SwipeItem>
            
                <SwipeItem>
                    <div class="swipeitem">
                    <div class="swipe__3">
                        <div class="content">
                            <img src="assets/Star.png" alt="">
                            <h3>Theo dõi lợi nhuận</h3>
                            <p>Theo dõi lợi nhuận của từng vé</p>
                        </div>
                    </div>
                    <div class="swipe__1">
                            <div class="content">
                                <img src="assets/Star.png" alt="">
                                <h3>Mua vé</h3>
                                <p>Mua vé của bạn để bắt đầu đầu tư</p>
                            </div>
                        </div>
                        <div class="swipe__2">
                            <div class="content">
                                <img src="assets/Star.png" alt="">
                                <h3>Chia sẻ</h3>
                                <p>Chia sẻ để xây dựng khoản lợi nhuận lớn mỗi ngày</p>
                            </div>
                        </div>
                    </div>
                </SwipeItem>
            
                <SwipeItem>
                    <div class="swipeitem">
                        <div class="swipe__3">
                            <div class="content">
                                <img src="assets/Star.png" alt="">
                                <h3>Chia sẻ</h3>
                                <p>Chia sẻ để xây dựng khoản lợi nhuận lớn mỗi ngày</p>
                            </div>
                        </div>
                        <div class="swipe__1">
                            <div class="content">
                                <img src="assets/Star.png" alt="">
                                <h3>Theo dõi lợi nhuận</h3>
                                <p>Theo dõi lợi nhuận của từng vé</p>
                            </div>
                        </div>
                        <div class="swipe__2">
                                <div class="content">
                                    <img src="assets/Star.png" alt="">
                                    <h3>Mua vé</h3>
                                    <p>Mua vé của bạn để bắt đầu đầu tư</p>
                                </div>
                            </div>
                    </div>
                </SwipeItem>
            
              </Swipe>
            </div>
            <div class="tab--btn">
                <button class="prev" on:click={prevSlide}>
                    <img src="assets/prev.png" alt="">
                </button>
                <button class="next" on:click={nextSlide}> 
                    <img src="assets/next.png" alt="">
                </button>
            </div>
        </div>
        <div class="slider__content">
            <p>Làm sao để bắt đầu?</p>
            <h3>Bắt đầu kiếm tiền Với những bước đơn giản</h3>
            <p>Bắt đầu với những bước đơn giản: Đầu tư ngay trong tầm bay bạn từ những bước click chuột đơn giản</p>
        </div>
    </div>
    <div class="reponsive">
        <div class="repon_content">
                <p>REPONSIVE</p>
                <h2>Tương thích với tất cả các loại màn hình</h2>
                <p>Trang web của chúng tôi được nâng cấp và có thể tương thích với các loại màn hình khác nhau như Iphone, Ipad,… Không gây khó chịu và nhiều hạn chế khi sử dụng so với các nền tảng khác.</p>
        </div>
        <img src="assets/112.png" alt="">
    </div>
    <div class="map">
        <h1 class="map__content">Mạng lưới của chúng tôi có mặt trên tất cả các quốc gia trên thế giới</h1>
        <div class="map__location">
            <div class="location--user">
                <img src="assets/location.png" alt="">
                <div class="users">
                <h2>7392</h2>
                <p>Người dùng</p>
                </div>
            </div>
            <div class="location--user">
                <img src="assets/ticket.png" alt="">
                <div class="users">
                <h2>3037</h2>
                <p>Vé trung bình mỗi ngày</p>
                </div>
            </div>
            <div class="location--user">
                <img src="assets/cup.png" alt="">
                <div class="users">
                <h2>80%</h2>
                <p>Người dùng chiến thắng</p>
                </div>    
            </div>
        </div>
    </div>
    <div class="makemoney">
        <h2>Kiếm tiền thật dễ dàng trên nền tảng Bitkingreturns</h2>
        <div class="btn">
            <button class="btn__join">Tham gia ngay</button>
            <button class="btn__find">Tìm hiểu thêm</button>
        </div>
    </div>

</main>

<style lang="scss">
    @import "../stylesheet/main.scss";
</style>