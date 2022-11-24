---
title: "[Git-Blog] 블로그 실행 관련 내용 정리"
permalink: /posts/github_blog
categories: 
  - github_blog
toc: true
toc_sticky: true
toc_label: "blog start info"
tags:
  - Git Blog
  - jekyll
---

## 블로그를 시작하면서..
블로그를 만들면서 배웠던 내용들을 정리해 보고자 합니다.

---

## GitHub Blog 를 선택한 이유

> 다양한 플랫폼의 블로그 서비스를 찾아보았습니다.  
> `naver`, `Tistory`, `brunch`, `Blogger`, `velog` 등등  
> 다양한 편의성을 제공하긴 했는데 뭔가 만들고 있다는 느낌보다는 가벼운 느낌을 지울 수가 없던 찰나 **`Github`**에서도 페이지를 구성해서 활용할 수 있음을 발견 이미 상당수 블로거들이 해당 페이지를 만들고 운영 중인 것을 확인할 수 있었습니다.
> <br>
>> ### GitHub Blog 장점
>> **`Github blog`**의 장점은 자유도가 높다는 점입니다.   
>> blog 개설부터 포스팅 및 각종 플러그인 등을 활용함에 있어 자유롭다는 부분이 마음에 들었습니다.
>> 수익창출이나 조회 수 등에 연연하지 않고 편하게 알고 있는 정보를 정리하고 기록하기에 최적화되어있다고 보았습니다.

---

## github.io

> google 검색에서 나온 [[SuperMemi Blog][1]{:target="_blank"}] 를 참조하여  작업했습니다.

[1]: https://supermemi.tistory.com/144 "Github Blog 시작하기"   

---

## Ruby 설치 // jekyll 설치

> [ruby 공식 홈페이지][2]{:target="_blank"}에서 가이드라인에 따라 진행  
window 환경에서는 [ruby installer][3]{:target="_blank"} 에서 다운로드 설치  
[별준 코딩][4]{:target="_blank"} 의 내용을 참고 하셔도 좋습니다.

[2]: https://www.ruby-lang.org/ko/documentation/installation/ "Ruby"
[3]: https://rubyinstaller.org/ "Ruby Installer"
[4]: https://junstar92.tistory.com/5 "별준 코딩, 루비설치"

---

## Serve 실행

1. window - cmd 실행   
2. blog 코드 경로에서 하위 문장 실행

```
bundle exec jekyll serve
```

실행결과
![bundle exec jekyll serve](/assets/images/posts/github_blog/bundle_exec_jekyll_serve.JPG)

---

## 참조

MarkDown Guide : <https://www.markdownguide.org>{:target="_blank"}  
MarkDown 사용법 : <https://heropy.blog/2017/09/30/markdown/>{:target="_blank"}   
Github Blog 시작하기 : <https://supermemi.tistory.com/144>{:target="_blank"}  
jekyll 사용법 : <https://velog.io/@eona1301>{:target="_blank"}
{: .notice}
