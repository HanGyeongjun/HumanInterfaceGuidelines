---
description: >-
  On Apple platforms, a material imparts translucency and blurring to a
  background, creating a sense of visual separation between foreground and
  background layers.
---

# Materials

{% hint style="info" %}
본 문서는 Apple의 Human Interface Guideline(이하 HIG) 문서를 한글로 번역한 것입니다. iOS 생태계 내에서 HIG를 읽으시는 분들이 번역본이 없어 불편함을 겪는 것을 알게 되었고, 이에 한글로 번역을 하게 되었습니다. iOS 커뮤니티 Async Swift에서 자율적으로 모인 9명이 함께 번역했으며, 일체의 상업적인 목적을 띄지 않습니다. 이 문서를 학습에 적극적으로 이용해 주시돼, 상업적인 용도로 이용하시는 것은 지양해 주시기 바랍니다. 감사합니다.
{% endhint %}

<figure><img src="../.gitbook/assets/foundations-materials-intro_2x (2).png" alt=""><figcaption></figcaption></figure>

## Introduction

**Apple 플랫폼에서 머터리얼은 배경에 반투명도와 흐림 효과를 부여하여 전경과 배경 레이어 사이에 시각적인 분리감을 만듭니다.**

머터리얼은 인터페이스에 시각적 흥미를 더하기 위해 생동감(Vibrancy)과 결합될 수 있습니다. 생동감은 텍스트, 심볼, 그리고 채우기 색 등 전경 위에 표시되는 콘텐츠에 적용되며, 머터리얼 뒤에서 색상을 앞으로 끌어와 심도감을 높입니다.

> 📝 **NOTE** 생동감은 macOS의 메뉴 및 iOS의 레이블 등 몇몇 컴포넌트에 기본으로 적용되어 있기 때문에 생동감을 적용한 화면을 표시하지 않더라도 모든 앱과 게임에 영향을 줄 수 있습니다.

***

## Best Practices

**시스템은 라이트 모드와 다크 모드에 모두 기본으로 적용되는 특정한 용도로 쓰이는 몇 가지 머터리얼을 정의합니다.** 또한 UI 컴포넌트에 적용할 수 있는 몇 가지 흐림(blur) 및 생동감 효과를 제공해 컴포넌트가 머터리얼과 잘 통합되고 돋보일 수 있게 도와줍니다. 시스템 정의 머터리얼과 효과를 사용하면 앱이나 게임에 네이티브한 느낌을 줄 수 있으며, 사람들이 앱 간 전환을 할 때 부드러운 전환 효과를 만들 수 있습니다.

**의미와 권장 용도에 따라 시스템 머터리얼과 효과를 선택하세요.** 시스템 설정이 형태와 동작을 변경할 수 있으므로 인터페이스 색상을 기반으로 머터리얼 또는 효과를 선택하지 않는 것이 좋습니다. 대신 특정 사용 사례에 맞는 머터리얼이나 스타일을 선택하세요. 예를 들어, macOS앱의 메뉴에서 [menu](https://developer.apple.com/documentation/appkit/nsvisualeffectview/material/menu) 머터리얼을 사용하고, iOS앱의 레이블에서 [label](https://developer.apple.com/documentation/uikit/uivibrancyeffectstyle/label) 생동감 스타일을 사용하고, tvOS앱의 적응형 전체 화면 배경에서 [prominent](https://developer.apple.com/documentation/uikit/uiblureffect/style/prominent) 머터리얼을 사용 것이 좋습니다.

**머터리얼 위에 선명한 색상만을 사용해 읽기 쉽게 하세요.** 시스템 정의된 선명한 색상을 사용할 때 다른 맥락에서 너무 어둡거나 밝게 보이고, 채도가 높거나 대비가 낮아 보이는 것에 대해 걱정할 필요는 없습니다. 예를 들어 iOS는 텍스트, 채우기, 글리프 및 구분선에 대해 동적 시스템 색상을 정의해 이러한 항목을 반투명 배경에서 멋지게 보이게 합니다. macOS에서 모든 표준 시스템 색상에는 생생한 버전이 있습니다. 가이드라인은 [Color](https://developer.apple.com/design/human-interface-guidelines/foundations/color)를 참고하세요.

**풀컬러 아이콘이 아닌 SF 기호를 사용하는 것을 검토해 주세요.** 풀컬러 이미지는 뷰의 배경과 충분한 대비가 되지 않아 배경이 반투명하면 부적절한 것처럼 보일 수 있습니다. 기호 및 인터페이스 아이콘은 동적 시스템 색상 및 생동감 효과와 함께 작동하며 모든 맥락에 적절합니다. 가이드라인은 [SF Symbols](https://papago.naver.net/apis/site/proxy?url=https%3A%2F%2Fdeveloper.apple.com%2Fdesign%2Fhuman-interface-guidelines%2Ffoundations%2Fsf-symbols)를 참고하세요.

**흐림 및 생동감 효과와 결합할 머터리얼을 선택할 때는 대비와 시각적 분리를 고려하세요.** 예를 들면 다음과 같습니다.

* 더 흐린(thicker) 머터리얼은 텍스트 및 작은 기능이 있는 기타 요소에 대해 더 나은 대비를 제공할 수 있습니다.
* 반투명성을 통해 백그라운드에 있는 콘텐츠를 시각적으로 확인할 수 있으므로 컨텍스트를 유지할 수 있습니다.

시스템은 콘텐츠를 방해하지 않고 깊이(depth)와 계층적 구조를 전달하기 위해 사용할 수 있는 몇 가지 머터리얼을 제공합니다. 가장 선명한(ultre thin) 것 부터 가장 흐린(ultra thick) 것 까지, 몇 개의 머터리얼은 화면 모드에 대해 적응형이고 일부 머터리얼은 항상 밝거나 어둡습니다. 선택한 머터리얼에 관계없이 그 위에 생동감이 없는(non-vibrant) 색상을 사용하는 것은 피해야 합니다.

개발자 가이드라인은 [UIBlurEffect.Style](https://papago.naver.net/apis/site/proxy?url=https%3A%2F%2Fdeveloper.apple.com%2Fdocumentation%2Fuikit%2Fuiblureffect%2Fstyle)를 참고하세요.

***

## **Platform considerations**

_Not supported in watchOS._

#### **iOS, iPadOS**

iOS 및 iPadOS는 각 머터리얼과 함께 작동하도록 특별히 설계된 레이블, 채우기 및 구분선에 대한 생동감 값을 정의합니다. 표준 시스템 색은 생동감(vibrant) 버전에서 사용할 수 없습니다.

레이블과 채우기 색은 각각 여러 수준의 생동감을 제공합니다. 구분선에는 하나의 수준이 있습니다. 수준의 이름은 요소와 배경 간의 상대적인 대비 정도를 나타냅니다. 기본 수준은 가장 높은 대비를 갖는 반면 수준4(존재하는 경우)는 가장 낮은 대비를 갖습니다.

수준4를 제외하고 모든 머터리얼의 레이블에 다음과 같은 생동감 값을 사용할 수 있습니다. 대비가 너무 낮기 때문에 가장 선명한(ultra thin) 머터리얼 위에 수준4의 생동감을 사용하지 않는 것이 좋습니다.

* [label](https://papago.naver.net/apis/site/proxy?url=https%3A%2F%2Fdeveloper.apple.com%2Fdocumentation%2Fuikit%2Fuivibrancyeffectstyle%2Flabel) (기본)
* [secondaryLabel](https://papago.naver.net/apis/site/proxy?url=https%3A%2F%2Fdeveloper.apple.com%2Fdocumentation%2Fuikit%2Fuivibrancyeffectstyle%2Fsecondarylabel)
* [tertiaryLabel](https://papago.naver.net/apis/site/proxy?url=https%3A%2F%2Fdeveloper.apple.com%2Fdocumentation%2Fuikit%2Fuivibrancyeffectstyle%2Ftertiarylabel)
* [quaternaryLabel](https://papago.naver.net/apis/site/proxy?url=https%3A%2F%2Fdeveloper.apple.com%2Fdocumentation%2Fuikit%2Fuivibrancyeffectstyle%2Fquaternarylabel)

모든 머터리얼을 채우는 데 다음과 같은 생동감 값을 사용할 수 있습니다.

* [fill](https://papago.naver.net/apis/site/proxy?url=https%3A%2F%2Fdeveloper.apple.com%2Fdocumentation%2Fuikit%2Fuivibrancyeffectstyle%2Ffill) (기본)
* [secondaryFill](https://papago.naver.net/apis/site/proxy?url=https%3A%2F%2Fdeveloper.apple.com%2Fdocumentation%2Fuikit%2Fuivibrancyeffectstyle%2Fsecondaryfill)
* [tertiaryFill](https://papago.naver.net/apis/site/proxy?url=https%3A%2F%2Fdeveloper.apple.com%2Fdocumentation%2Fuikit%2Fuivibrancyeffectstyle%2Ftertiaryfill)

시스템은 구분선에 대해 모든 머터리얼에서 잘 작동하는 하나의 기본 생동감 값을 제공합니다.

#### macOS

macOS는 모든 표준 색상에 대한 생동감 효과를 제공하며 인터페이스에 사용되는 투명도, 흐림 및 생동감 효과의 양을 정의하는 머터리얼을 제공합니다. 시스템은 각각 지정된 용도를 가진 몇 가지 표준 머터리얼을 제공합니다. 예를 들어 창, 메뉴, 팝오버, 사이드바, 제목 표시줄 등의 기본 모양과 어울리는 머터리얼을 선택할 수 있습니다. 개발자 가이드라인은 [NSVisualEffectView.Material](https://papago.naver.net/apis/site/proxy?url=https%3A%2F%2Fdeveloper.apple.com%2Fdocumentation%2Fappkit%2Fnsvisualeffectview%2Fmaterial)를 참고하세요.

![라이트 모드](../.gitbook/assets/macos-light-appearance\_2x.png)

![다크 모드](../.gitbook/assets/macos-dark-appearance\_2x.png)

**사용자 지정 뷰 및 컨트롤에서 생동감 효과를 표시할 때를 선택하세요.** 구성 및 시스템 설정에 따라 시스템 뷰 및 컨트롤은 생동감 효과를 사용하여 전경 콘텐츠를 어떤 배경에서도 돋보이게 만듭니다. 다양한 상황에서 인터페이스를 테스트하여 생동감 효과가 외관과 커뮤니케이션을 향상시키는 경우를 찾는 것이 좋습니다.

**인터페이스 디자인을 보완하는 배경 혼합 모드를 선택하세요.** macOS는 배경 콘텐츠를 혼합하는 두 가지 모드(창 뒤 및 창 내)를 정의합니다. 개발자 가이드라인은 [NSVisualEffectBlendingMode](https://papago.naver.net/apis/site/proxy?url=https%3A%2F%2Fdeveloper.apple.com%2Fdocumentation%2Fappkit%2Fnsvisualeffectblendingmode)를 참고하세요.

![창 뒤 블렌딩](../.gitbook/assets/macos-behind-window-blending\_2x.png)

**창 뒤 블렌딩.(Behind-window blending)** 이 모드에서는 창 뒤에 있는 콘텐츠가 표시되어 사람들이 앱 또는 게임을 둘러싼 일부 컨텍스트를 유지하도록 돕습니다. 메뉴, 시트 및 사이드바와 같은 구성 요소는 이 모드를 자동으로 사용합니다.

![창 내 블렌딩](../.gitbook/assets/macos-in-window-blending\_2x.png)

**창 내 블렌딩.(In-window blending)** 이 모드를 사용하면 창 콘텐츠가 또다른 다른 창 구성 요소를 통해 표시됩니다. 예를 들어 툴바는 이 모드를 사용해 창 콘텐츠가 툴바 아래에서 스크롤될 때 사람들에게 연속성을 제공할 수 있습니다.

#### tvOS

**더 선명하고 반투명한 머터리얼을 선택해** 콘텐츠**를 강조하고 밝음을 느낄 수 있도록 하세요.** 어두운 머터리얼은 그림자를 숨기는 경향이 있어 깊이를 줄이고 내용을 명확하게 구분하기 어렵게 만듭니다. 더 무거운 느낌을 주거나 내용이 더 오래된 것을 제안하려면 어두운 머터리얼을 사용하는 것을 고려할 수 있습니다.

예를 들어, 다음과 같은 방법으로 시스템 머터리얼을 사용하는 것을 고려해 보세요.

| Material    | Recommended for                                                                        | Adaptive behavior                                                                                            |
| ----------- | -------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------ |
| Prominent   | Full-screen backgrounds                                                                | Displays the extra light material in the light appearance and the extra dark material in the dark appearance |
| Regular     | Overlay views that partially obscure onscreen content                                  | Displays the light material in the light appearance and the dark material in the dark appearance             |
| Extra light | Full-screen views that require a light color scheme                                    | –                                                                                                            |
| Light       | Overlay views that partially obscure onscreen content and require a light color scheme | –                                                                                                            |
| Extra dark  | Full-screen views that require a dark color scheme                                     | –                                                                                                            |
| Dark        | Overlay views that partially obscure onscreen content and require a dark color scheme  | –                                                                                                            |

***

## **Resources**

#### **Related**

* [Color](https://developer.apple.com/design/human-interface-guidelines/foundations/color)
* [Accessibility](https://developer.apple.com/design/human-interface-guidelines/foundations/accessibility)

#### **Developer documentation**

* [Material — SwiftUI](https://developer.apple.com/documentation/swiftui/material/)
* [UIVisualEffectView — UIKit](https://developer.apple.com/documentation/uikit/uivisualeffectview)
* [NSVisualEffectView — AppKit](https://developer.apple.com/documentation/appkit/nsvisualeffectview)

#### **Videos**

*   ****[**What's New in iOS Design** WWDC 2019](https://developer.apple.com/videos/play/wwdc2019/808/)

    ![](https://devimages-cdn.apple.com/wwdc-services/images/48/3272/3272\_wide\_250x141\_2x.jpg)
