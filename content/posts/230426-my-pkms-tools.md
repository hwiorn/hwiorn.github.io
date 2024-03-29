+++
title = "나의 지식관리 도구"
author = ["hwiorn"]
expiryDate = 2999-01-01
lastmod = 2023-04-27T11:19:48+09:00
tags = ["pkms"]
categories = ["pkms"]
draft = true
+++

<div class="ox-hugo-toc toc has-section-numbers">

<div class="heading">Table of Contents</div>

- <span class="section-num">1</span> [사용 도구](#사용-도구)
    - <span class="section-num">1.1</span> [Emacs](#emacs)
    - <span class="section-num">1.2</span> [Syncthing (기기간 파일 동기화)](#syncthing--기기간-파일-동기화)
    - <span class="section-num">1.3</span> [Git Annex (파일관리)](#git-annex--파일관리)
    - <span class="section-num">1.4</span> [Jabref (문헌관리)](#jabref--문헌관리)
    - <span class="section-num">1.5</span> [Joplin (스크랩)](#joplin--스크랩)
- <span class="section-num">2</span> [캡쳐](#캡쳐)
- <span class="section-num">3</span> [노트 작성](#노트-작성)
- <span class="section-num">4</span> [노트 정리](#노트-정리)

</div>
<!--endtoc-->

2023년 4월 26일 기준 PKMS에 사용하는 툴 목록이다.

현재 주력으로 사용하는 툴은 Emacs이며, 주 OS는 Linux 환경[^fn:1]이고, 모바일은
아이폰[^fn:2]을, 이북리더는 오닉스포크3(안드로이드)를 사용한다.


## <span class="section-num">1</span> 사용 도구 {#사용-도구}

나는 주로 도구의 경우 주력으로 사용하면, 대체품을 함께 사용하는 경향이 있다.

{{< figure src="/ox-hugo/f6748e1b-5550-4257-8a92-afc69f3cb925.excalidraw.svg" >}}


### <span class="section-num">1.1</span> Emacs {#emacs}

지식 관리의 주력 프로그램이며, org-roam을 기반으로 지식관리를 하고 있다.
org-roam은 org-mode에 roam의 기능 일부(백링크)를 가져온 것으로, 성능이 빨라서
쓰고 있다.

org-roam을 사용하게 끔 만들었던, org-roam-ui는 현재는 노트 작성 워크플로를
개선해나가면서, 현재는 거의 사용하지 않게 되었다.


### <span class="section-num">1.2</span> Syncthing (기기간 파일 동기화) {#syncthing--기기간-파일-동기화}

iOS, Android, PC간 동기화를 할 수 있으며, 주로 공부하거나 봐야하는 문서들을
모바일 기기간 동기화하며, 다 본 문서의 경우, git-annex로 이동시킨다.

Syncthing은 파일 동기화를 해줄 뿐, 버전관리나 백업의 용도로는 부적합하며, 다른
기기에서 서로 작업한 경우, 동기화가 되지 않으면 충돌이 생기므로, 주의해야 한다.


### <span class="section-num">1.3</span> Git Annex (파일관리) {#git-annex--파일관리}

파일 버전관리, 백업, 동기화로 사용한다.

백업은 google drive 2TB와 Backblaze B2로 이중화를 하고 있다.

드랍박스, 아이클라우드, 구글드라이브, Synology Drive 순으로 사용하고 있었으나,
아래와 같은 이슈가 있어, PC간 파일 관리는 git annex를 사용 중이다.(모바일에서는
사용할 수 없음)

-   드랍박스: 제일 무난하지만, 정책 변경과 비용이 비싼 점.
-   아이클라우드: 맥을 사용할 때, 대안이 없다 시피하지만 느리고 파일 사라짐 이슈가
    존재. 현재는 사진 백업 용도.
-   구글드라이브: 리눅스에서 클라이언트 사용 불가.
-   Synology Drive: 파일을 삭제해도 디렉토리가 살아나는 이상 현상이 존재함.

현재는 Synology는 개인 NAS로 사용하고 있으며, 아이클라우드는 가족 사진 공유 및
백업 용도, 구글 드라이브는 git annex에서 API를 이용한 백업 용도로 사용 중.


### <span class="section-num">1.4</span> Jabref (문헌관리) {#jabref--문헌관리}

원래는 Zotero를 사용했으나, BibTeX 포맷을 사용하기 번거로운 점[^fn:3]과 pdf를
외부로 저장하는 방식의 번거로움[^fn:4], 다른 기기에서 세팅하기 번거로움[^fn:5]
등에 따라 포기했다.

JabRef는 기능적으로 떨어지나 bibtex과 biblatex 포맷을 바로 수정한다는 점에서
관리 목적상 사용하고 있다.


### <span class="section-num">1.5</span> Joplin (스크랩) {#joplin--스크랩}

에버노트에서 이전해왔으며, 그 전에는 업무보고나 초안을 작성할 때,
사용하였다.

스크랩은 joplin 을 사용한다. 지금은 거의 사용하지 않고 있다. 커뮤니티 사이트에
올라와서, 특정 토픽에 관심 있는 경우에는 스크랩[^fn:6]을 한다.


## <span class="section-num">2</span> 캡쳐 {#캡쳐}

-   일반 임시 메모: Kate(메모장)
    -   Kate는 KDE의 메모장(보다 notepad++와 유사)이며, 임시 메모를 작성할 때
        사용한다.
-   아날로그: 포켓수첩[^fn:7]
    -   포켓 수첩을 항상 갖고 다니면서 책의 내용을 메모하거나, 생각나는 것들을
        적는다.
-   메신져: 텔레그램
    -   파일 보존기간이 무제한(용량과 속도는 제한)이고, 확장성이 높은 메신져라서
        추후에 보고자 할 때 보관 용도로 사용한다.
    -   아이폰이나 안드로이드에서도 PDF나 텍스트 등을 다른 기기에서 보고자 할때,
        유용하다.
-   PC: org-roam 캡쳐(Emacs)
-   Web 하이라이팅/메모: hypothes.is
    -   하이라이팅과 메모를 동시에 수행할 수 있음
-   Youtube 메모: reclipped, org-media-note(Emacs)
    -   reclipped는 웹 서비스로 제공되며, 앱은 따로 존재하지 않지만 북마크릿을 통해
        reclipped 서비스로 이동하여 메모를 할 수가 있다.
-   전자책
    -   사용하는 서비스는 킨들[^fn:8]과 리디북스[^fn:9]이며, 메모를 주로 사용하고, 스크립트를 통해 org 파일로 만들고 있다.


## <span class="section-num">3</span> 노트 작성 {#노트-작성}

-   PC: Emacs
-   iOS: 안함


## <span class="section-num">4</span> 노트 정리 {#노트-정리}

-   PC: Emacs
-   iOS: 안함

[^fn:1]: Android, iOS, Windows 프로그램 개발을 했었기 때문에, 맥과 윈도우 역시
    무리없이 사용할수 있지만, 아무래도 오픈소스인 Linux 배포판 만큼 어떤 이슈를
    수정하고 가다듬는다는 느낌을 많이 못받는 것 같다.
[^fn:2]: 주로 Emacs와 Linux를 쓰는 사용자는 안드로이드 기반을 사용하기 때문에,
    iOS의 경우 관련 자료나 워크플로에 대한 글들이 많이 존재하지는 않는다.
[^fn:3]: BetterBibTeX 플러그인을 사용하면 bibtex 파일로 뽑아내어 사용할수 있지만,
    bibtex의 변경사항이 Zotero의 collection으로 다시 반영되지 않는다.
[^fn:4]: zotfile 플러그인을 사용해야 하고, 드랍박스나 webdav를 사용한다면 규칙을
    통일시켜주는 등의 설정이 추가로 필요하다.
[^fn:5]: 현재는 모바일 버전이 나왔지만, zotero 클라우드를 통해 PDF를 관리하지
    않는다면 다른 기기에서 함께 사용하기가 번거롭다.
[^fn:6]: 경험담이나 해결 방법 등의 정보가 올라오지만 글쓴이의 변심이나
    공격때문인지 삭제되는 경우가 종종 있었다.
[^fn:7]: 포켓 수첩은 양지사 PD90을 썼지만, 1달이상 쓰면 겉표지가 말그대로
    쪼개진다. 그래서 지금은 미도리 패스포트 형태의 가죽 수첩을 사용한다. 속지는
    한동안 미도리 호환을 쓰다가 지금은 다이소의 500원 수첩을 끼워서 사용하고 있다.
[^fn:8]: 킨들의 경우 메모를 하기 위해서 하이라이트가 필요한데, 하이라이트를 많이
    할 경우 저작권 정책에 의해 제약이 걸린다. 출판사마다 다른데 약 10~20% 정도이고,
    모든 하이라이트를 가져올 수 없는 것으로 보인다.
[^fn:9]: 리디북스의 메모와 하이라이트는 epub 파일만 지원하고, PDF는 전혀 지원하지
    않는다. 그래서 PDF의 경우 구글북스 등을 통해 구매하여 DRM을 해제하고 보는 사람
    도 있지만, 나는 굳이 그렇게 할 필요를 못느꼈다.