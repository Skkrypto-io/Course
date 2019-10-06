# [BASIC-0](https://github.com/Skkrypto-io/Course)
Course info for the Skkrypto


# **Welcome!**

반갑습니다! 여러분은 스크립토 학회의 일원으로서 BASIC 팀의 교육과정을 거치게 됩니다.    
이번 BASIC 교육과정은 플랫폼에 상관없이 블록체인의 기본 컴포넌트들을 빡세게 몸소 체험하여 스캠 프로젝트들을 보면 몸에 거부반응이 와서 걸러낼 정도의 전문성을 함양하는 것을 목표로 하고 있습니다. 


# 참고사항

- 입문은 파이썬이나 자바스크립트로 시작할 건데 블록체인을 정말 심각하게 들어가거나 암호학 라이브러리를 사용해야하는 경우 **Rust나 GO, 심하면 C++** 까지 들어갈 수 있으니
미리 과정을 익히시면서 배워두시는 게 좋습니다. 

- 학교에서 legacy라고 불려도 조금은 말이 될 듯할 안전성이 지루할 정도로 검증된 폐급 윈도우 비주얼 스튜디오와 C와 C++의 혼종 syntax를 가르치는 경우와 달리 여기는 오픈소스에 기여하는 개발자가 최신화가 발빠르게 진행되고 있는 리눅스나 맥, 오픈소스 툴들을 사용합니다.
그러니 윈도우를 사용하시면 현재 기술들이 서포트 따위 거의 신경도 안쓰는 운영체제라 어려움이 있을 수도 있다는 점 알아두세요!

- REST API를 한번 구현해보시거나 json-rpc에 대한 이해도가 높아야 합니다.

# Curriculum

커리큘럼은 project-based learning(PBL), flip-learning으로 진행되며 아래에 있는 6개의 프로젝트들을 수행해가며 질문이나 같이 논의해야 할 사항을 매주 토요일에 만나서 처리합니다.
단, 학회원들의 실력과 수요에 따라 내용이 크게 달라질 수 있습니다. 프로젝트의 예상 기간은 약 1달에서 2달 정도로 잡고 있으며 python을 주로 쓸 예정입니다. 

1. lab0: [Damien van Flymen](https://medium.com/@vanflymen/learn-blockchains-by-building-one-117428612f46)의 blockchain tutorial
  - 학습목표: 블록체인을 전체적으로 흝어서 어떻게 블록체인이 변경이 불가능한 데이터를 생성하고 이를 공유하는 지 알아봅시다.
  - Project: blockchain.py에 docstring 만들어서 documentation 만들어보기.
  - Extra: dvf/blockchain에 documentation으로 기여해보기.
  
2. lab1: ECDSA와 비대칭키 알고리즘
  - 학습목표: 비대칭키가 어떻게 그냥 암호넣어서 암호화시키는 것과 달리 자신임을 인증시켜주는 지 알아보고 이를 사용해봅시다.
  - Project: [이더리움/비트코인 주소]() 만들기
  - Extra: satoshi labs가 제시하는 스펙을 참고하여 [hdkey wallet]() 만들기
  
3. lab2: Trie와 embedded key-value database
  - 학습목표: 어떻게 블록 하나가 블록체인의 모든 데이터를 하나의 해쉬만으로 검증이 가능하게 하는지 알아보고 LevelDB와 RocksDB는 어떻게 구동하는지 알아봅시다.
  - Project: state 만들기
  - Extra: trie가 적용된 state database 만들기

4. lab3: p2p connection using python
  - 학습목표: p2p가 어떻게 소통하는지 알아보고 이를 활용하는 프레임워크인 libp2p에 대해서 알아봅시다.
  - Project: 파이썬 파일 하나로 아주 간단히 ping만 보내는 p2p client 만들어보기
  - Extra: libp2p로 채팅앱 만들어보기(Rust/Go/javascript) * python은 아직 개발중이라 불가능합니다.
  
5. lab4: RPC api 설계
  - json-rpc에 대해 이해하고 
  - Project: leveldb를 이용해 state를 저장하는 블록체인 state-machine을 만든 다음 REST나 jsonrpc를 이용해서 tx_pool에 리퀘스트를 쌓고 block_confirmation time이 지날 때 마다 처리하는 솔로 노드를 만들어봅시다.
  - Extra: p2p로 블록 공유 가능한 블록체인 만들기
  
6. lab5: Consensus and finality
  - 학습목표: uncle/aunt block에 대해 이해하고 여러개의 블록들이 다음 블록의 후보로 정해졌을 때 어떤 블록을 택하게 하는 finality gadget에 대해 알아봅시다.
  - Project: 마이닝 할 때 마다 자기 블록과 uncle block을 비교해서 finalized block 선택하는 프로세스 만들기
  - Extra: 기존에 만든 state-machine에 연동시켜보세요!
  

# FAQ

### 만약에 이 프로젝트를 통과하지 못하면 어떻게 하죠?

**저희는 주어진 기한 내에 프로젝트를 끝내라고 강요하지 않습니다.** 여유롭게 준비가 되면 skkrypto01@gmail.com으로 자기 계정에서 만든 깃허브 리포지토리 링크를 보내주세요.


### 만약에 이 프로젝트를 통과하면 어떻게 되나요?

나중에 해커톤이나 학회 주도의 프로젝트 진행에 참여하실 때 참고사항이 될 수 있으며 나중에 운영진으로 활동하여 멘토로서 다음 기수를 가르치실 수 있습니다.

### 다른 교육과정은 없나요?

BASIC에서 제공하는 교육과정 외에도 이더리움 기반 dapp 외 실질적인 서비스들을 만들고 싶다는 의견에 따라 AP 팀에서 댑 커리큘럼을 만들 수 있습니다. 
이외 노드 인프라의 경우 SRE, 컨센서스나 finality를 향상시키거나 이를 proof assistant로 수학적으로 증명해보고 싶으신 분들은 CORE 팀에서 멘토나 운영진이 되는 사람들이 
프로젝트를 만들 계획입니다. 프로젝트 모듈 식으로 운영되려고 하니 학습자 마음대로 학습목표에 맞게 골라 들으시면 됩니다.


# 표절

Skkrypto 개발 팀은 교육과정이 모두 오픈소스로 진행되는 만큼 표절을 용납할 수 없습니다. 프로젝트에 표절이 발견 됬을 시 프로젝트를 했다고 인정할 수 없습니다. 표절에 관한 건은 피드백으로 어디가 표절인지 알려드린 다음 
출처를 밝히셔야 패스하실 수 있다는 점 알아두세요.


# 질문이나 도움

질문이나 도움은 Skkrypto의 공식 슬랙 방의 `#개발팀`채널이나 슬랙에 있는 제 계정으로 DM 보내주시면 됩니다.
