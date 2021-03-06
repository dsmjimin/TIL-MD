# Git_flow & Github_flow 알아보기



### Git_flow

아래는 Git_flow를 설명할 때 빠질 수 없는 사진이다.

![git-flow_overall_graph](https://techblog.woowahan.com/wp-content/uploads/img/2017-10-30/git-flow_overall_graph.png)

#### Git flow는 5가지 브런치를 사용한다.

##### ❗	feature >> develop >> release >> hotfix >> main 순서	❗

* **main**(=master) : **master보다는 main이라는 이름**으로 더 많이 사용 중이다. 프로젝트 시작부터 끝까지 유지되는 **메인 브런치**다.
  * 개발을 다 끝내고 제품으로 출시할 수 있을 때 이용하는 브런치다.
* **develop** : main 브런치와 함께 끝까지 유지되는 **메인 브런치**로, 다음 출시 버전을 개발하는 브런치다.
  * 참고로 위 사진에서 볼 수 있듯이 main 브런치보다 develop 브런치가 좀 더 활발히 이용된다.
* **feature** : 직접적으로 기능을 개발하는 브런치이며 **다수의 브런치**를 만들 수 있다. 여러번 만들어지고 사라지는 **보조 브런치**다.
  * 팀프로젝트에서 여러 feature 브런치를 만들어 각자 개발을 하고 develop 브런치로 넘기거나,
    혼자서 여러 부분을 개발하며 브런치를 늘릴 수 있다.
  * 프로젝트를 진행하며 가장 많이 사용하는 브런치다. 개인적으로 feature 브런치를 이용해
    세밀하게 개발 부분을 나눠 정리하면 좋다고 생각한다.
* **release** : develop에서 개발한 것들을 main 브런치로 넘길 때 사용된다. **보조 브런치**다.
  * 보통 feature 브런치에서 남겼던 주석을 지우고 main으로 넘긴다.
    * 필자는 release 이름을 [SemVer 방식](https://github.com/dsmjimin/TIL-MD/blob/main/Node.js%20Package%20Version.md)으로  정한다.
* **hotfix** : 출시 버전에서 출시 버전에서 발생한 버그를 수정하기 위해 만든다. **보조 브런치**다.
  * 필자는 아직까지 사용해 본 적이 없지만, 생각을 얘기해보자면 지속적으로 유지보수를 하는 프로젝트에 주로 사용할듯하다.

### Github_flow

![Git TextBook | 깃브랜치&gt;전략](https://git.jiny.dev/gitflow/img/gitflow_02.png)

#### Github flow는 2가지 브런치만 사용한다.

main 브런치와 feature 브런치 두 가지만 사용한다. Git_flow가 Github에서는 사용하기 애매하여 나온 전략이라고 알고 있다.

흐름은 main 브런치에서 feature 브런치를 하나 생성하여 개발을 진행 후 해당 기능의 개발이 끝나면 다시 main 브런치로 넘기는 것(merge)이다. Git flow처럼 다수의 브런치를 만들 수 있기 때문에 역시나 프로젝트 진행 파트를 팀원이 나눌 수 있다.

보조 브런치가 feature 하나이고, develop 브런치가 없는 만큼 feature에서 main으로 넘길 때에는 신중하게 해야한다. Github에서 사용하는 만큼 Pull Request 기능을 적극적으로 활용하여 사용하는 것이 좋다.









release : 

> https://techblog.woowahan.com/2553/

📢 Git_flow branch 설명 부분 제외 검색 없이 작성 중.

📢 오타, 오류 지적 환영!
