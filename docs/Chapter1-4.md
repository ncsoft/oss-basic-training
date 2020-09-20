<!--
Chapter 1. 저작권과 오픈소스 라이선스
4. 주요 오픈소스 라이선스
-->

##  주요 오픈소스 라이선스
###  오픈소스 라이선스는 약 <span style="color: blue">2,500개</span> 정도 있다고 합니다.
<br>

###  그 중에서 상위 10개의 라이선스가 전체의 93%를 차지하고 있습니다.
|순위|라이선스 명|2018년|2019년|리스크|
|:--:|:--:|:--:|:--:|:--:|
|1|MIT License|38%|32%|Low|
|2|GNU General Public License v2.0 (GPL 2.0)|14%|18%|<span style="color: orange">High</span>|
|3|Apache License 2.0|13%|14%|Low|
|4|GNU General Public License v3.0 (GPL 3.0)|6%|7%|<span style="color: orange">High</span>|
|5|BSD 3-Clause License (BSD 3-clause “New” or ”Revised” License)|5%|6%|Low|
|6|Internet Systems Consortium License (ISC License)|6%|5%|Medium|
|7|Artistic License|3%|4%|Medium|
|8|GNU Library or Lesser General Public License v2.1 (LGPL 2.1)|3%|4%|<span style="color: orange">High</span>|
|9|GNU Library or Lesser General Public License v3.0 (LGPL 3.0)|1%|2%|<span style="color: orange">High</span>|
|10|Eclipse Public License (EPL)|1%|1%|Medium|
|기타|GNU Affero General Public License (AGPL)|1% 미만|1% 미만|<span style="color: orange">Very High</span>|
<br>

###  오픈소스 라이선스는 소스코드 공개의무 강도에 따라 크게 Permissive 라이선스와 Copyleft 라이선스로 구분할 수 있습니다.
*  Permissive 라이선스: Easy Mode
*  Copyleft 라이선스: Hard Mode
<br>

###  Permissive 라이선스는 의무사항이 많지 않아서 상대적으로 준수하기가 쉬운 라이선스입니다. <span style="color: blue">일반적으로 저작권 표시, 라이선스 고지 등의 고지 의무만 준수하면 됩니다.</span>
*  MIT
   *  MIT에서 해당 대학의 공학도들을 돕기 위해 개발한 라이선스
   *  라이선스 및 저작권 명시 (고지문)
   *  예: Bootstrap, Angular.js, X-Windows 
*  Apache
   *  아파치 재단의 모든 소프트웨어에 적용되는 라이선스
   *  BSD 라이선스 의무사항 
   *  특허 보복 조항  +  <span style="color: blue">GPL 2.0으로 배포되는 코드와는 결합 불가능</span>
   *  예: Android, Hadoop
*  BSD
   *  소스코드를 공개하지 않아도 되는 대표적인 라이선스
   *  저작권 명시 (고지문), 저작권자 동의 없이 저작권자 이름 사용 제한
   *  예: Nginx
<br>

###  <span style="color: blue">Copyleft 라이선스는 Permissive 라이선스에 비해 의무사항이 복잡하고 까다롭습니다.</span> Copyleft란 Copyright(저작권)에 반대되는 개념으로 저작권에 기반을 두고 사용을 제한하는 것이 아니라 저작권을 기반으로 정보 공유를 강화하려는 자유 소프트웨어 운동에서 주장하는 개념입니다.
*  <span style="color: green">Copyleft 로고: Copyright의 ©를 뒤집어 놓은 형태</span>
<br>

###  Copyleft 라이선스의 오픈소스가 포함되어 있는 파생저작물을 배포하려면 <span style="color: blue">원래의 오픈소스 라이선스와 동일한 라이선스로만 배포해야 하는 의무사항</span>이 있습니다.
*  파생저작물 (GPL) > <span style="color: green">배포 시 라이선스 변경 불가능 (한번 Copyleft는 영원한 Copyleft !)</span> > GPL
*  파생저작물 (BSD) > 배포 시 라이선스 변경 가능 > MIT, Apache, GPL
<br>

###  Copyleft 라이선스에 따라서는 <span style="color: blue">사용자가 만든 파생저작물의 소스코드도 함께 배포할 것을 요구</span>하기도 합니다.
*  내가 공유한 소스를 이용해서 다른 프로그램을 만들면 너도 그 프로그램의 소스를 공유해야 해.
*  그..래.. 알겠어...
<br>

###  GPL 라이선스의 오픈소스는 해당 바이너리 전체의 모든 소스코드를 공개해야 하는 의무가 있습니다.
*  클라이언트 (SDK) (SDK) (SDK) (SDK) (SDK) (GPL 코드)  Dynamic Linking이라도  <  (GPL 코드)
*  클라이언트 (SDK) (SDK) (SDK) (SDK) (SDK) (GPL 코드)  모두 GPL化
<br>

###  LGPL 라이선스의 오픈소스를 수정해서 사용하거나 Static Linking으로 사용하게 되면 해당 바이너리 전체의 오브젝트 코드를 공개해야 하는 의무가 있습니다.
*  자사 소스코드, Static Linkinig(a), LGPL 오픈소스, 실행파일
*  자사 소스코드, 실행파일, Dynamic Linking(.so), LGPL 오픈소스, Library
<br>

###  AGPL 라이선스의 오픈소스는 웹 서비스를 통해 서비스를 제공하는 것도 배포로 보기 때문에 <span style="color: blue">오픈소스 사용고지 및 수정해서 사용했다면 수정된 소스의 소스코드를 공개해야 하는 의무가 있습니다.</span>
*  서버, AGPL이 아닌 것 > 웹 서비스 <span style="color: blue">(배포로 보지 않음)</span>
*  서버, AGPL > 웹 서비스 <span style="color: orange">(오픈소스 사용고지 및 소스의 공개의무 발생)</span>
<br>

###  Copyleft 라이선스와 Permissive 라이선스의 주요 의무사항을 비교해 보면 다음과 같습니다.
<br>

####  <span style="color: green">강한 Copyleft</span>
*  <span style="color: green">소스코드 공개의무 : 강함</span>
*  <span style="color: green">주요 라이선스</span>
   *  <span style="color: green">GNU General Public License v2.0 (GPL 2.0)</span>
   *  <span style="color: green">GNU General Public License v3.0 (GPL 3.0)</span>
   *  <span style="color: green">GNU Affero General Public License (AGPL)</span>
*  <span style="color: green">주요 의무사항</span>
   *  <span style="color: green">사용 시 소스코드 공개</span>
   *  <span style="color: green">재배포 시 라이선스 변경 금지</span>
<br>

####  약한 Copyleft
*  소스코드 공개의무 : 약한
*  주요 라이선스
   *  GNU Library or Lesser General Public License v2.1 (LGPL 2.1)
   *  GNU Library or Lesser General Public License v3.0 (LGPL 3.0)
   *  Eclipse Public License (EPL)
   *  Artistic License
*  주요 의무사항
   *  수정하거나 정적 링킹하여 사용 시 오브젝트 코드 공개
<br>

####  Permissive
*  소스코드 공개의무 : 없음
*  주요 라이선스
   *  MIT License
   *  Apache License 2.0
   *  BSD 3-Clause License 
   *  Internet Systems Consortium License (ISC)
*  주요 의무사항
   *  사용 사실과 저작권자에 대한 고지
<br>

