[Adblock Plus 2.0]
! Title: 乘风 视频过滤规则
! Version: 202307122
! Expires: 1 day
! Homepage: https://github.com/xinggsf/Adblock-Plus-Rule/issues

! 屏蔽P2P
yy.com,le.com##+js(nowebrtc)
||tracker.$xhr,websocket,script,ping
||p2p.$xhr,websocket,ping,domain=~huya.com|~binance.com

v.youku.com##.control-phonewatch,#right-title-ad-banner, .kui-watermark-0
!m.youku.com,v.youku.com##+js(nano-stb, r--,, 0.02)
m.youku.com,v.youku.com##+js(m3u-prune,'',/^https:\/\/[\w\.]+ott\.cibntv\.net.+?\.m3u8\?/)
atm.youku.com
cad.youku.com
@@||mmstat.com^$domain=youku.com
||cibntv.net/youku/$media
||valipl.cp31.ott.cibntv.net/$media
!|https://static.youku.com/index/js/ikuAdapterNew.js
||sealine.youku.com/yk/*callback=adpagesdk$script

iqiyi.com##.black-screen[data-cupid="adblock-blackscreen"]
iqiyi.com##div[data-adzone],#block-V
iqiyi.com##+js(set, Object.prototype.parseXML, noopFunc)
iqiyi.com##+js(set, Object.prototype.blackscreenDuration, 1)
m.iqiyi.com##+js(set, Object.prototype.adPlayerId, '')
||static.iqiyi.com/js/common/mars_v.js$script
||iqiyi.com/videos/other/202$xmlhttprequest
||71edge.com/videos/other/202$xmlhttprequest
||iqiyipic.com/image/20*_100000$image
apisgame.iqiyi.com
static.g.iqiyi.com
||ssports.iqiyi.com/json/shop/shopInfo
||ssports.iqiyi.com/app/$media,object-subrequest
show.ssports.com


bilibili.com##.ad-report, .ad-floor
bilibili.com##.gg-floor-module,#slide_ad,a[href^="//cm.bilibili.com"]
||api.bilibili.com/x/web-show/res/loc?pf=$~script
||hdslb.com/bfs/sycp/creative_img/$image
cm.bilibili.com

acfun.cn##.pause-display-container,#ad-comment,#ad-player-view
||aixifan.com/static/*/appGuide/

cctv.com###bgAd_div
!||imall.cctv.com/$subdocument
bjcathay.com

pptv.com##.advView-two,#p-mark
synacast.com
de.as.pptv.com
||g.pptv.com/game/$subdocument
||osswc.pplive.cn/cccms/$image

||cmvideo.cn/v1/iflyad/delivery$media,domain=miguvideo.com
! 风行网： fun.tv
pub.funshion.com

||relive.vodfile.m1905.com/video/qiantie202$media

@@||tb.mgtv.com/sdk/*/ad-sdk.
ad-survey.com
||video.da.mgtv.com/$media
||da.mgtv.com/mediafiles/wiad_creative/$image

@@||js.tv.itc.cn/gg.seed.js
||css.tv.itc.cn/m/img/player/dlBanner.$image
||data.vod.itc.cn/*&prod=ad&$media
||api.my.tv.sohu.com/wm/getads.do?
||aty.sohu.com/
adpushup.com
||go.sohu.com/
||tv.sohu.com/upload/csad/admaster/$image
tv.sohu.com##.x-dl-shake.x-download-panel, #playerBar > div.area ~a
17173.com###vjs-ad-on-pause
||log1.17173.com/
||17173.com/batch_show?ads=
||17173.com/if/$script,subdocument

le.com##+js(set, isAdLoaded, true)
*/letv-gug/$media,object-subrequest,xhr
||letvimg.com/$object,xhr
||letvimg.com/*_gugwl/$image
||js.letvcdn.com/*_banner_$script
||banana.le.com/
adxvip.com
behe.com
biddingx.com
cr-nielsen.com
fancyapi.com
ipinyou.com
kejet.net
||jd.com/$domain=le.com
ulmdb.cn
xelements.cn
yoyi.com.cn
zhiziyun.com
le.com##.min_pause_img
! 视频水印
le.com##.hv_wm_logo

cctv.com,www.douyu.com##+js(aeld,/visibilitychange|pagehide/)
douyu.com##+js(set, RTCPeerConnection.prototype.addTrack, noopFunc)
||douyucdn.cn/adxdsp/$image
wan.douyu.com
douyu.com##.Title-ad, .DropMenuList-ad, .DropPane-ad
douyu.com,huya.com##a[href^="https://g.wan."]
huya.com###hy-ad,#hy-ab,#huya-ab
g.huya.com
||msstatic.com/huya/*/p2plib.js$script

www.ted.com##.gm-fp-body .justify-center.tracking-tightest
||onetrust.
litix.io
||stripe.com^$script,domain=~nextdns.io|~obsidian.md

youtube.com##.masthead-ad-control, .ad-div, .pyv-afc-ads-container, #promotion-shelf
*_ad_$media,domain=youtube.com,3p
youtube.com##ytd-video-masthead-ad-advertiser-info-renderer, ytm-promoted-sparkles-web-renderer, ytd-promoted-sparkles-web-renderer
youtube.com,youtube-nocookie.com##+js(json-prune, [].playerResponse.adPlacements [].playerResponse.playerAds playerResponse.adPlacements playerResponse.playerAds adPlacements playerAds)
youtube.com,youtube-nocookie.com##+js(set, ytInitialPlayerResponse.adPlacements, undefined)
youtube.com,youtube-nocookie.com##+js(set, playerResponse.adPlacements, undefined)
||youtube.com/pagead/
||youtube.com/ptracking?
||google.*/pagead/
||gstatic.com/shopping?

*/preroll/$media,domain=91porn.com
91p20.space
waust.at

||btsow.mom/app/jav$image
jads.co
|https://tellme.pw/go/jav$popup
|https://$script,subdocument,popup,3p,domain=btsow.mom|dandanzan10.top|dandanzan.*|nunuyingyuan.com|nunuyy5.org|rarbgprx.org
!btsow.mom##+js(aeld, click, popunder)
!btsow.*##body>div[id]:last-child>a:only-child
! 2022 https://rarbgprx.org
statsy.net
||dyncdn.me/static/20/js/showads.js$script
||dyncdn.me/static/20/js/expla$script

age.tv,agemys.net##+js(noeval-if, devtoolsDetector)
||toutiaoimg.com/origin/$image,domain=agemys.net|acgndmku.com|subaibaiys.com

dandanzan.com,dandanzan10.top,nunuyy5.org##+js(set,RTCPeerConnection,null)
dandanzan.com,dandanzan10.top,nunuyy5.org##+js(set,webkitRTCPeerConnection,null)
dandanzan.com,dandanzan10.top,nunuyy5.org##+js(set,mozRTCPeerConnection,null)
dandanzan.com,dandanzan10.top,nunuyy5.org#@#+js(nowebrtc)
dandanzan.com,dandanzan10.top,nunuyy5.org##.gm-fp-body video:style(max-height:100%!important)
wpadmngr.com
|https://static.cloudflareinsights.com/beacon.min.js^$xhr,script
||nunuyingyuan.tk/serviceworker.js^$script
||nunuyy.cf/serviceworker.js^$script

www.sbdm.net##.dplayer-web-fullscreen-fix .billhao-head-image, .dplayer-web-fullscreen-fix #topnav
aqours.today
chushoushijian.cn
z4a.net
www.sbdm.net##.ads_all:remove()
|https://dd-static.jd.com/ddimg/jfs/t1/173245/15/28822/346324/62fcb4b0Eb437d047/136a1e04890320b8.jpg$image,domain=subaibaiys.com
yatu.tv##.dplayer-web-fullscreen-fix #tburl,#loadtop,[id^=myas],#myds1,#daohang
yatu.tv,yhdm15.com##+js(set,document.oncontextmenu,trueFunc)
onenews.vip
quickapp.cn
v4dwkcv.com
weizhenwx.com
youle55.com
||www.yatu.tv:2082/image/*.gif^$image
||www.yatu.tv:2082/m/images/$image

||nooen.com^$popup
bixinlive.com
orgaorg.com
quandangdang.net
stgowan.com
