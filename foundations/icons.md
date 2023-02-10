---
description: >-
  An effective icon is a graphic asset that expresses a single concept in ways
  people instantly understand.
---

# Icons



{% hint style="info" %}
본 문서는 Apple의 Human Interface Guideline(이하 HIG) 문서를 한글로 번역한 것입니다. iOS 생태계 내에서 HIG를 읽으시는 분들이 번역본이 없어 불편함을 겪는 것을 알게 되었고, 이에 한글로 번역을 하게 되었습니다. iOS 커뮤니티 Async Swift에서 자율적으로 모인 9명이 함께 번역했으며, 일체의 상업적인 목적을 띄지 않습니다. 이 문서를 학습에 적극적으로 이용해 주시돼, 상업적인 용도로 이용하시는 것은 지양해 주시기 바랍니다. 감사합니다.
{% endhint %}

<figure><img src="../.gitbook/assets/foundations-icons-intro_2x.png" alt=""><figcaption></figcaption></figure>

## Introduction

**잘 디자인된 아이콘은 사용 목적과 기능을 사람들이 즉시 이해할 수 있도록 표현한 그래픽 요소입니다.**

아이콘은 앱과 게임에서 사용되어 사용자들에게 해당 아이콘을 통해 어떤 작업과 기능을 수행할 수 있는지 쉽게 알려줄 수 있어야 합니다. [App icons](https://developer.apple.com/design/human-interface-guidelines/foundations/app-icons) 은 음영, 질감 및 강조 표시와 같은 풍부한 시각적 표현 방식을 사용하여 앱의 개성을 나타낼 수 있는 반면, 아이콘은 일반적으로 간결한 모양과 색상을 사용해 그 의미를 전달합니다.

아이콘은 글리프 또는 템플릿 이미지라고도 하는데 SF Symbols 앱에서 기호를 선택하여 있는 그대로 사용하거나 필요에 맞게 사용자가 디자인할 수 있습니다. 아이콘과 기호는 모두 검은색과 선명한 색상을 사용하여 모양을 디자인합니다. 시스템은 각 이미지의 검은색 영역에 다른 색상을 적용할 수 있습니다. 가이드라인은 [SF Symbols를](https://developer.apple.com/design/human-interface-guidelines/foundations/sf-symbols) 참고하세요.



## Best practices

**사람들이 아이콘을 쉽게 이해할 수 있고, 최대한 단순하게 디자인해야 합니다.** 너무 많은 세부 정보를 아이콘에 표현하면 사람들은 혼란스러울 수 있습니다. 대다수의 사람들이 빠르게 알아볼 수 있는 단순하고 보편적인 디자인을 하는 것이 좋습니다. 일반적으로 아이콘은 작업이나 해당 콘텐츠에 직접적으로 연관된 메타포(metaphors)로 표현될 때 가장 좋습니다.

*   역자설명

    은유(metaphors)라고 합니다. 예를 들어 사람들이 기존에 학습되어 있거나 친숙한 아이콘을 사용하면 해당 아이콘에 대한 설명이 없더라도 자연스럽게 해당 아이콘의 기능을 떠올릴 수 있습니다.

**앱의 모든 아이콘에서 시각적인 일관성을 유지하세요.** 커스텀 아이콘 또는 시스템이 제공하는 아이콘과 함께 사용하든지 상관없이 앱의 모든 아이콘은 크기, 세부 디테일, 획 두께 및 원근감을 동일하게 사용해야 합니다. 아이콘의 시각적 가중치에 따라 다른 아이콘과 일치하도록 크기를 조정해야 할 수 있습니다.

{% embed url="https://img1.daumcdn.net/thumb/R1280x0/?fname=http%3A//t1.daumcdn.net/brunch/service/user/eUo8/image/BXZZ976nNHt61sMxbJdrLvC-9RY.png" %}

**일반적으로 아이콘과 가까운 텍스트의 가중치(시각적 무게)를 통일시킵니다.** 앱에서 아이콘이나 텍스트를 강조할 필요가 없는 경우, 동일한 가중치를 사용해 디자인하면 콘텐츠에 일관된 모양과 시각적 무게감을 줄 수 있습니다.

**필요한 경우, 광학 정렬(시각적 정렬)을 맞추기 위해 사용자 정의 아이콘에 패딩을 추가합니다.** 아이콘 중, 비대칭인 아이콘은 광학 대신 비율로 중앙에 배치되면 불균형적이게 보일 수 있습니다. 예를 들어, 아래에 표시된 다운로드 아이콘은 위쪽보다 아래쪽에 더 많은 시각적 가중치가 있으므로 비율상 중앙에 있으면 너무 낮게 보여 패딩을 통해 위쪽으로 조정할 수 있습니다.

{% embed url="https://img1.daumcdn.net/thumb/R1280x0/?fname=http%3A//t1.daumcdn.net/brunch/service/user/eUo8/image/B4XN_s7MLZs03wCX89em-1Z1VQU.png" %}

이러한 경우 아이콘이 시각적으로 중앙에 배치하기 위해 아이콘의 위치를 약간 조정할 수 있습니다. 아이콘 주위에 패딩을 통해 중앙에 배치하여 시각적으로 중앙에 배치할 수 있습니다.

{% embed url="https://img1.daumcdn.net/thumb/R1280x0/?fname=http%3A//t1.daumcdn.net/brunch/service/user/eUo8/image/PFUpthaibJXqgkQwHTCVYOE9mhw.png" %}

시각적인 중심에 대한 위치 조정은 매우 사소하지만 앱의 모양에 큰 영향을 미칠 수 있습니다.

{% embed url="https://img1.daumcdn.net/thumb/R1280x0/?fname=http%3A//t1.daumcdn.net/brunch/service/user/eUo8/image/k4BsCKHqgp9g9D2e6ffDnrcH_cA.png" %}

**필요한 경우에만 활성화 상태의 아이콘 디자인을 제공하세요.** 애플이 제공하는 아이콘(ex.SF Symbol)은 활성화 및 비활성화 상태를 따로 디자인할 필요가 없이 자동으로 제공됩니다. 하지만 iOS 도구 모음 및 탐색 모음(사이드바, iOS 탭 표시줄 및 macOS 도구 모음)은 활성화 상태의 아이콘을 제공하지 않아 앱의 악센트 컬러(강조 색상)를 사용하거나 배경을 추가하여 활성화 상태를 사용자에게 전달할 수 있습니다.

{% embed url="https://img1.daumcdn.net/thumb/R1280x0/?fname=http%3A//t1.daumcdn.net/brunch/service/user/eUo8/image/kjzBGblLbDlRMy_u_T3Yu05XR6U.png" %}

반대로 iOS 도구 모음과 탐색 모음은 활성화 아이콘을 제공하지 않으므로 각 아이콘의 채워진 버전과 채워지지 않은 버전을 모두 만들어야 합니다.

{% embed url="https://img1.daumcdn.net/thumb/R1280x0/?fname=http%3A//t1.daumcdn.net/brunch/service/user/eUo8/image/BNzSUFIY48Pc30GHl3D6AirYSwc.png" %}

**포괄적(Inclusion)인 아이콘 디자인을 만드는 것이 좋습니다.** 특정 성별이 떠오르는 아이콘보다 모든 사람을 포괄적으로 설명할 수 있는 아이콘을 사용하는 것이 좋습니다. 가이드라인은 [Inclusion을](https://developer.apple.com/design/human-interface-guidelines/foundations/inclusion) 참고하세요.

**의미를 전달하는 데 꼭 필요한 경우에만 디자인에 텍스트를 포함하세요.** 아이콘의 의미를 직접적으로 전달해야 할 때에는 텍스트가 포함된 아이콘을 사용할 수 있습니다. 또한 아이콘에 텍스트를 표시해야 하는 경우 해당 문자를 사용 국가에 맞춰 현지화해야 합니다. 한 줄 정도의 텍스트를 통해 어떤 것을 제안해야 하는 경우에 사람들이 오해하지 않게 추상적인(포괄적인) 표현을 사용하고, 읽는 방향이 오른쪽에서 왼쪽일 때 반대 방향의 아이콘도 함께 제공해야 합니다. 가이드라인은 [Right to left을](https://developer.apple.com/design/human-interface-guidelines/foundations/right-to-left) 참고하세요.

{% embed url="https://img1.daumcdn.net/thumb/R1280x0/?fname=http%3A//t1.daumcdn.net/brunch/service/user/eUo8/image/w17-g-X5DchIIbebU46ac-AL17I.png" %}

**커스텀 아이콘을 새로 만드는 경우, PDF 또는 SVG와 같은 벡터 형식을 사용하세요.** 시스템은 고해상도의 디스플레이로 벡터 기반 아이콘의 크기를 자동으로 조정하여 인터페이스에 보여줍니다. 하지만 음영, 텍스처 및 하이라이트와 같은 효과를 포함하는 앱 아이콘 및 PNG 이미지는 크기 조정을 지원하지 않으므로 PNG 기반 아이콘은 해상도에 따른 여러 버전을 제공해야 합니다. 또는 사용자 정의 SF 기호를 만들 수도 있습니다. 가이드라인은 [SF Symbols를](https://developer.apple.com/design/human-interface-guidelines/foundations/sf-symbols) 참고하세요.

*   역자설명

    SVG 벡터 형식의 그래픽은 함수로 계산된 그래픽으로 확장 또는 축소 시 형태가 변하지 않습니다. 픽셀 형태로 표현된 PNG의 경우 확장 또는 축소 시 픽셀이 깨질 수 있습니다.

**커스텀 아이콘에 대한 대체 텍스트 레이블(Label)을 제공하는 것이 좋습니다.** 대체 텍스트 레이블(Label) 또는 아이콘에 대한 설명은 인터페이스에서는 보이지 않지만 보이스 오버(VoiceOver)가 화면에 표시되는 내용을 청각적으로 설명하도록 하여 시각 장애인의 앱 사용을 돕습니다. 가이드라인은 [Content descriptions](https://developer.apple.com/design/human-interface-guidelines/foundations/accessibility/#content-descriptions)을 참고하세요.

*   역자설명

    VoiceOver 보이스 오버, 손쉬운 사용과 같은 접근성을 위한 도구입니다. 이미지 또는 아이콘에  대체 텍스트 레이블을 지정해 놓으면 보이스 오버가 시각 장애인 분들을 위해 해당 아이콘 및 이미지를 설명해 줍니다.

**아이콘에 Apple 하드웨어 제품의 형태를 사용하지 않도록 합니다.** 하드웨어의 디자인은 자주 변경될 수 있으며, 사람들이 헷갈리지 않게 아이콘 및 기타 콘텐츠를 새로운 디자인으로 바꿔줘야 합니다. [Apple Design Resources](https://developer.apple.com/design/resources/) 또는 다양한 Apple 제품을 나타내는 SF 기호에서 사용할 수 있는 이미지만 사용하세요.



## Platform considerations

_No additional considerations for iOS, iPadOS, tvOS, or watchOS._

### macOS

#### Document icons

macOS 앱에서 제공하는 유형의 파일이라면 자동으로 문서 아이콘을 생성할 수 있습니다. 일반적으로 오른쪽 위 모서리가 접힌 종이 조각처럼 보입니다. 이 독특한 형태는 아이콘 크기가 작은 경우에도 사람들이 문서 아이콘을 다른 콘텐츠와 구별하는 데 도움을 줍니다.

macOS 앱에서 제공하는 유형의 파일이 아니면 앱 아이콘, 파일 확장자를 함께 표시하여 아이콘을 생성합니다. 예를 들어 미리 보기는 시스템 생성한 문서 아이콘을 사용하여 JPG 파일을 나타냅니다.

{% embed url="https://img1.daumcdn.net/thumb/R1280x0/?fname=http%3A//t1.daumcdn.net/brunch/service/user/eUo8/image/Xynl0OgxfY7WCQ7rcaglQ4qxP28.png" %}

경우에 따라 앱에서 파일 형식을 나타내는 문서 아이콘 세트를 만들어두면, 구별하기 편리합니다. 예를 들어 Xcode는 커스텀 문서 아이콘을 사용하여 사람들이 프로젝트, AR 개체 및 Swift 코드 파일을 구별할 수 있도록 합니다.

{% embed url="https://img1.daumcdn.net/thumb/R1280x0/?fname=http%3A//t1.daumcdn.net/brunch/service/user/eUo8/image/fDZpl2AKpntMq8aaDZXWGkEouEk.png" %}

커스텀 문서 아이콘을 생성하기 위해 배경 채우기, 중앙 이미지 및 텍스트의 조합을 사용할 수 있습니다. macOS 11부터 시스템은 이러한 요소를 적절히 합성해 문서 아이콘 모양으로 합성합니다.

{% embed url="https://img1.daumcdn.net/thumb/R1280x0/?fname=http%3A//t1.daumcdn.net/brunch/service/user/eUo8/image/vCXjRsovowje4kr5gEH_EKg55k8.png" %}

[Apple Design Resources는](https://developer.apple.com/design/resources/#macos-apps) 커스텀 문서 아이콘을 생성하는 데 사용할 수 있는 템플릿을 제공합니다. 이 템플릿을 사용할 때 아래 가이드라인을 참고하세요.

**문서 유형을 명확하게 전달할 수 있는 단순한 이미지를 사용합니다.** 배경, 중앙 이미지 또는 둘 다를 사용하든, 복잡하지 않은 모양과 고유한 색상으로 단순한 형태로 디자인하는 게 좋습니다. 문서 아이콘은 16x16픽셀만큼 작게 표시할 수 있으므로 모든 크기에서 사용자들이 쉽게 알 수 있는 디자인을 만들어야 합니다.

**하나의 잘 디자인된 배경 이미지를 사용하면, 사람들이 문서의 유형을 이해하는데 도움이 될 수 있습니다.** 예를 들어 Xcode와 TextEdit는 모두 중앙 이미지가 아닌 배경 이미지만을 사용합니다.

{% embed url="https://img1.daumcdn.net/thumb/R1280x0/?fname=http%3A//t1.daumcdn.net/brunch/service/user/eUo8/image/JxUIGzTDI_ySzfee7FzEvGBSgsU.png" %}

**작은 사이즈의 문서아이콘은 최대한 단순하게 디자인하세요.** 아이콘 디자인에 따라 큰 사이즈에서는 세부 정보가 흐릿하게 보이고, 작은 사이즈에서는 사람들이 알아보기 어려울 수 있습니다. 예를 들어, 커스텀한 하트 문서 아이콘의 격자선이 명확하게 보이도록 하기 위해 더 적은 수의 선을 사용하고 선을 더욱 굵게 표현할 수 있습니다. 16x16픽셀 크기에서는 그리드를 제거해 단순하게 만들 수 있습니다.

{% embed url="https://img1.daumcdn.net/thumb/R1280x0/?fname=http%3A//t1.daumcdn.net/brunch/service/user/eUo8/image/ejFb767z-unsGDJz55U-X_NVBDc.png" %}

**배경의 오른쪽 상단 모서리에 중요한 콘텐츠를 배치하지 않는 것이 좋습니다.** 시스템은 문서 아이콘 형태에 맞게 이미지를 자동으로 자르고 흰색 접힌 모서리 형태로 변경합니다. 이후 아래 크기의 배경 이미지 세트를 만듭니다.

* 512x512픽셀 @1x, 1024x1024픽셀 @2x
* 256x256픽셀 @1x, 512x512픽셀 @2x
* 128x128픽셀 @1x, 256x256픽셀 @2x
* 32x32픽셀 @1x, 64x64픽셀 @2x
* 16x16픽셀 @1x, 32x32픽셀 @2x

**문서의 유형을 쉽게 전달할 수 있는 이미지가 있는 경우, 문서를 나타내는 중앙 이미지를 만드는 것이 좋습니다.** 모든 크기에서 명확하고 알아볼 수 있는 단순하고 모호하지 않은 이미지를 디자인합니다. 중앙 이미지는 전체 문서 아이콘 캔버스 크기의 절반 사이즈가 좋습니다. 예를 들어 32x32픽셀 문서 아이콘의 중앙 이미지를 만들려면 16x16픽셀 크기의 이미지 캔버스를 사용합니다. 아래 크기의 중앙 이미지를 제공할 수 있습니다.

* 256x256픽셀 @1x, 512x512픽셀 @2x
* 128x128픽셀 @1x, 256x256픽셀 @2x
* 32x32픽셀 @1x, 64x64픽셀 @2x
* 16x16픽셀 @1x, 32x32픽셀 @2x

**이미지 캔버스의 약 10%의 여백을 측정하고, 여백 안에 이미지의 대부분을 나타냅니다.** 이미지의 일부가 광학 정렬을 위해 이 여백으로 밖으로 확장될 수 있지만 이미지가 캔버스의 약 80%를 차지할 때 가장 좋습니다. 예를 들어, 256x256픽셀 캔버스에 있는 대부분의 중앙 이미지는 205x205픽셀 크기의 영역을 사용하는 것이 좋습니다.

{% embed url="https://img1.daumcdn.net/thumb/R1280x0/?fname=http%3A//t1.daumcdn.net/brunch/service/user/eUo8/image/oK0zKXq_l0ahAnHMbrFZjJV_FpI.png" %}

**사람들이 문서 유형을 이해하는 데 도움이 되는 경우, 간결한 용어를 사용하는 것이 좋습니다.** 기본적으로 시스템은 문서 아이콘의 아래쪽 가장자리에 문서의 확장자를 표시하지만 확장자가 익숙하지 않은 경우 더 이해하기 쉬운 간결한 용어를 사용할 수 있습니다. 예를 들어 SceneKit 파일의 문서 아이콘은 파일 확장명 ‘scn’ 대신 ‘scene’이라는 용어를 사용합니다. 시스템은 문서 아이콘에 맞게 텍스트의 크기를 자동으로 조정하므로 작은 크기에서도 읽을 수 있을 만큼 짧은 용어를 사용해야 합니다. 기본적으로 시스템은 텍스트의 모든 문자를 대문자로 표시합니다.

{% embed url="https://img1.daumcdn.net/thumb/R1280x0/?fname=http%3A//t1.daumcdn.net/brunch/service/user/eUo8/image/Ab4ZbkAyfV6RtKg_8z3-KXPHP5A.png" %}

## **Resources**

#### **Related**

* [App icons](https://developer.apple.com/design/human-interface-guidelines/foundations/app-icons)
* [SF Symbols](https://developer.apple.com/design/human-interface-guidelines/foundations/sf-symbols)

#### **Videos**

*   ****[**Designing Glyphs** WWDC 2017](https://developer.apple.com/videos/play/wwdc2017/823/)

    ![https://devimages-cdn.apple.com/wwdc-services/images/7/1914/1914\_wide\_250x141\_2x.jpg](https://devimages-cdn.apple.com/wwdc-services/images/7/1914/1914\_wide\_250x141\_2x.jpg)
