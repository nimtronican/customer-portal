---

copyright:

  years: 1994, 2018

lastupdated: "2018-09-05"

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:tip: .tip}
{:screen: .screen}
{:new_window: target="_blank"}


# 알림 구독
{: #cp_bpnotifications}

때때로 조치가 필요한 {{site.data.keyword.BluSoftlayer_notm}} 인프라에서 이벤트가 발생합니다. 일부는 계획되지 않고 일부는 계획된 유지보수 활동으로, 최상의 상태에서 {{site.data.keyword.BluSoftlayer_notm}} 인프라 작동을 유지해야 합니다. 고객은 최대한 이벤트에서 격리되지만 장비를 오프라인으로 전환해야 하는 경우도 있습니다. 고객에게 미치는 영향에 관계없이, 항상 투명하고 시기 적절하며 정보를 제공해야 합니다.
{:shortdesc}

클라우드 경헝을 제어해야 하므로 유지보수 활동에 대한 시기 적절한 정보가 필요합니다. 이 정보를 얻기 위해 고객 포털에서 알림을 구독할 수 있습니다. {{site.data.keyword.BluSoftlayer_notm}} 인프라는 다음 유형의 중요 작동 이벤트에 대한 EMS(Event Management System) 알림 프로세스를 사용합니다.
* 계획되지 않은 인프라 문제: 특정 고객을 위한 지정된 조건에서 가동 중단의 원인이 될 수 있는 문제
* 계획된 서비스 유지보수: 최적의 상태에서 인프라 작동을 유지해야 하는 유지보수
* 열린 지원 티켓: 계정에서 열린 티켓에 대해 구독한 사용자 경보

{{site.data.keyword.BluSoftlayer_notm}} 인프라 알림은 다음 주요 원칙을 고수하여 클라우드 환경을 위해 디자인되었습니다.
* 고객 포털을 통해 자동화됨
* 증가하는 대형 커뮤니티에 도달하도록 스케일링 가능함
* 이벤트로 영향을 받은 고객 및 리소스의 서브세트만 식별하기 위해 {{site.data.keyword.BluSoftlayer_notm}} 인프라를 사용하도록 대상이 지정됨

알림 시스템을 완전히 작동시키려면 프로세스를 구독하십시오. 알림 시스템이 필요한 중요 환경을 보유하고 있는 경우 24시간의 적용 범위도 설정하십시오.


## 알림 시간 제어 정책
{: #cp_bpgsnotiftimpol}

{{site.data.keyword.BluSoftlayer_notm}} 인프라 기간은 이벤트가 계획되지 않은 인프라 문제이거나 계획된 유지보수인지 또는 스케줄된 유지보수인지에 따라 보류 중인 이벤트 전에 사용자에게 차이점을 제공합니다. 일반적으로 {{site.data.keyword.BluSoftlayer_notm}} 인프라 정책은 더 큰 영향을 줄 수 있는 추가 문제 발생의 위험성을 제거하거나 최소화하기 위해 가능한 빨리 문제점을 해결하는 것입니다. 이는 계획된 유지보수의 경우에도 짧은 사전 알림으로만 수행되기도 함을 의미합니다.

### 정책 개요
{: #cp_bpgsnotifpolover}

각 섹션에 설명된 다음 유형의 가동 중단 또는 문제점에 대한 알림이 수신됩니다.

#### 계획되지 않은 문제 또는 가동 중단
{{site.data.keyword.BluSoftlayer_notm}} 인프라는 정보가 알려지는 즉시 인프라 범위, 임시 해결책 또는 해결 예측에 대한 정보와 함께 가능한 빨리 영향을 받은 고객과 통신합니다. 시기 적절한 통신은 긴급 상황에 대해 계획하는 데 필요한 정보를 제공하고 {{site.data.keyword.BluSoftlayer_notm}} 인프라에서 문제를 해결하고 있음을 보장합니다.

#### 스케줄된 유지보수
{{site.data.keyword.BluSoftlayer_notm}} 인프라는 이벤트 전에 스케줄된 유지보수에 대한 알림을 제공합니다. {{site.data.keyword.BluSoftlayer_notm}} 인프라 유지보수가 긴급한 경우가 있으며, 이에 따라 더욱 짧은 사전 알림이 발생하게 됩니다. 항상 목표는 긴급 상황을 위해 계획할 수 있도록 사전 알림의 적절한 시간 제공과 일반적으로 전체적인 안전성을 개선시키는 인프라 업그레이드, 향상 또는 필요한 기능 추가 간에 이상적인 균형을 찾는 것입니다.

#### 보안 취약성
{{site.data.keyword.BluSoftlayer_notm}} 인프라는 영향을 받은 영역을 격리하고 취약성을 차단하기 위해 패치를 작성하고 부수적인 기능이 영향을 받지 않는지 패치를 테스트합니다. 때때로 이 작업은 영향을 받은 기술 파트를 제공할 수 있는 다른 공급업체와 함께 수행됩니다. 일반적으로 보안 패치를 위해 퍼블릭 알림 금지가 있으며 퍼블릭을 보호하도록 짧게 지속되지만 좀 더 짧은 사전 알림이 요구됩니다. 퍼블릭에서 문제를 알게 되기 전에 {{site.data.keyword.BluSoftlayer_notm}} 인프라가 영향을 받은 인프라 전반에 패치를 구현합니다. 그렇지 않으면 위험이 증가됩니다. 취약성이 빨리 닫힐수록 위험이 제거됩니다. 이는 보안 문제에 짧은 알림 창이 필요함을 의미합니다.

보안상 결함이 좀 더 빈번한 대상 중 하나는 가상 인프라 소프트웨어입니다. {{site.data.keyword.BluSoftlayer_notm}} 인프라는 Virtual Server 오퍼링을 제공하기 위해 인기 있는 오픈 소스 및 파트너 기술을 사용합니다. 보안 수정사항을 구현하기 위해 가상 인프라 소프트웨어를 실행하는 고객 서버는 오프라인으로 설정되어 패치하고 환경을 다시 부팅해야 할 수 있으며, 이로 인해 중단이 발생합니다. 고객에게 미치는 영향을 최소화하기 위해 {{site.data.keyword.BluSoftlayer_notm}} 인프라는 최근에 가상 인프라에 대한 알림 프로세스에 대한 개선사항(향상된 통신)을 구현하였습니다. 특정 시작 시간과 각 Pod에 90분 창으로 고객에게 알림을 제공하며, 이를 통해 중단 시간이 줄어 들고 시간이 좀 더 정확하게 지정되어 준비하는 데 도움이 됩니다. 알림 시스템은 90분 창 전에 가장 자주 발생하는 알림 시스템은 {{site.data.keyword.BluSoftlayer_notm}} 인프라에서 특정 호스트가 제공되는 즉시 고객에게 알리도록 하여 각 계정에 대한 유지보수를 격리합니다.

#### 영향을 받은 다중 POD 또는 데이터 센터
{{site.data.keyword.BluSoftlayer_notm}} 인프라는 더 큰 2차 영향을 피하기 위해 수정사항을 구현하는 데 긴급 상황이 발생하지 않는 한 좀 더 길게 사전 알림 제공하려고 합니다.


## 구독자에게 이벤트 알림 추가
{: #cp_bpaddsub2eventnotcp}

IBM 고객은 관리형 인프라 서비스에 대해 IBM과 계약을 체결하고 {{site.data.keyword.BluSoftlayer_notm}} 인프라에 실행되는 클라우드 서비스 관련 계약을 맺거나 {{site.data.keyword.BluSoftlayer_notm}} 인프라 서비스와의 직접적인 계약을 체결함으로써 점점 더 {{site.data.keyword.BluSoftlayer_notm}} IaaS(Infrastructure as a Service)에 의존합니다. 클라우드 서비스에 인프라가 포함되면 앞의 절에서 설명된 대로 SoftLayer 계정 사용자가 알림을 받도록 권한이 부여됩니다. 일부 경우에는 인프라 서비스의 운영이나 지원에 참여하는 IBM 계정 또는 관리 서비스 팀이 자신의 SoftLayer 계정에 액세스하는 것을 원하지 않을 수도 있습니다. 계정에 대한 권한 없이 알림을 받을 수 있도록 사용자가 구독자(예: IBM 직원)의 목록을 지정할 수 있는 새 기능이 {{site.data.keyword.BluSoftlayer_notm}} 인프라 고객 지원에 추가되었습니다.

구독자의 목록을 지정하려면 마스터 사용자는 고객 포털 계정에 로그인하고 다음 단계를 수행할 수 있습니다.
1. 메뉴에서 **지원** > **이벤트**를 클릭하십시오.
2. 이벤트 유형을 선택하여 구독자를 추가하십시오.
2. 팝업 창에서 이메일 주소를 추가하십시오. 이메일 주소는 IBM이거나 비IBM일 수 있습니다.
3. **작성**을 클릭하십시오.

추가 구독자로 추가된 이메일 주소는 계획된 이벤트 알림 및 계획되지 않은 이벤트 알림을 받고 지원 티켓을 엽니다. 알림에는 기술 세부사항이 추가되었으므로 사용자는 구독자를 추가할 때 이를 고려해야 합니다. 알림에 대한 자세한 기술 특성으로 인해 예상 등록자는 {{site.data.keyword.BluSoftlayer_notm}} 인프라 환경에 영향을 주는 방식에 대해 자세하게 이해할 수 있는 사용자가 됩니다. 알림의 세부사항을 기반으로 한 잠재적 클라이언트 영향을 이해할 수 없는 수신인을 구독하는 것은 역효과가 발생할 수 있고 권장하지 않습니다.
