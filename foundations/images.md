---
description: >-
  To make sure your artwork looks great on all devices you support, learn how
  the system displays content on the screen and how to deliver art at the
  appropriate scale factors.
---

# Images

{% hint style="info" %}
본 문서는 Apple의 Human Interface Guideline(이하 HIG) 문서를 한글로 번역한 것입니다. iOS 생태계 내에서 HIG를 읽으시는 분들이 번역본이 없어 불편함을 겪는 것을 알게 되었고, 이에 한글로 번역을 하게 되었습니다. iOS 커뮤니티 Async Swift에서 자율적으로 모인 9명이 함께 번역했으며, 일체의 상업적인 목적을 띄지 않습니다. 이 문서를 학습에 적극적으로 이용해 주시돼, 상업적인 용도로 이용하시는 것은 지양해 주시기 바랍니다. 감사합니다.
{% endhint %}

![](../.gitbook/assets/foundations-images-intro\_2x.png)

## Introduction

**지원하는 모든 기기에서 아트웍 디자인이 멋지게 보이도록 하기 위해 화면에 콘텐츠를 표시하는 방법과 적절한 배율로 디자인하는 방법을 알아봅시다.**

****

## Scale factors

*   역자설명

    스케일 팩터는 이미지의 화질을 결정합니다. 이미지는 정사각형 모양의 작은 상자(픽셀) 안에 각 색상이 채워지고, 픽셀이 여러 개 모여 하나의 이미지를 구성합니다. 그래서 같은 크기의 이미지라도 픽셀의 개수가 많을수록 이미지가 섬세하고 정교하게 보입니다.

모든 플랫폼은 디스플레이의 포인트 측정을 기반으로 하는 좌표 시스템을 사용합니다. 표준 해상도 디스플레이는 1:1 픽셀 밀도를 가지며 여기서 1픽셀은 1포인트와 같습니다. 고해상도 디스플레이는 2:1 또는 3:1과 같이 픽셀 밀도가 더 높습니다. 2:1 밀도는 배율이 2이고 3:1 밀도는 배율이 3입니다. 픽셀 밀도가 높기 때문에 고해상도 디스플레이에는 더 많은 픽셀이 포함된 이미지가 필요합니다.

*   역자설명

    1:1 픽셀 밀도를 ‘@1x’라고도 하며, 2:1 픽셀 밀도는 ’@2x’, 3:1 픽셀 밀도’@3x’라고 일컫기도 합니다.

{% embed url="https://img1.daumcdn.net/thumb/R1280x0/?fname=http%3A//t1.daumcdn.net/brunch/service/user/eUo8/image/MR_4kTGdGjD5e40gONaFS8PjXX4.png" %}



## Formats

다양한 유형의 이미지를 생성할 때 다음 권장 사항을 고려하세요.

{% embed url="https://img1.daumcdn.net/thumb/R1280x0/?fname=http%3A//t1.daumcdn.net/brunch/service/user/eUo8/image/mGnRYlkmSSHpJzqfXFTV6fajESU.png" %}

*   역자설명

    이미지의 형식의 종류는 다음과 같습니다.

    * 비트맵 이미지 (Bitmap), 픽셀 안에 색상정보가 기억되는 방식의 파일형태로, 해상도를 줄였다 늘렸다 하면 화질이 깨질 우려가 있습니다. 고정되어 있는 이미지에 주로 사용됩니다. (Ex. PNG, JPG 등)
    * 벡터 이미지 (Vector), 획의 이동 정보가 기억되는 방식의 파일형태로, 해상도를 줄였다 늘렸다 해도 화질이 깨질 우려가 없습니다. 일러스트를 통한 아트워크를 만들었을 때나 반응형에서 작동하는 아이콘 이미지에 주로 사용됩니다. (Ex. PDF, SVG 등)



## Best practices

**지원하는 모든 기기에서 앱의 아트워크에 고해상도 이미지를 제공하세요.** 각 이미지의 픽셀 수에 특정 배율을 곱하면 됩니다. 프로젝트의 에셋(asset) 카탈로그에 각 이미지를 추가할 때 파일 이름에 "@1x", "@2x" 또는 "@3x"를 추가하여 스케일 팩터를 구분합니다. 다음 값을 가이드라인으로 사용하세요. 추가 축척 비율은 [Layout](https://developer.apple.com/design/human-interface-guidelines/foundations/layout) 을 참고하세요.

{% embed url="https://img1.daumcdn.net/thumb/R1280x0/?fname=http%3A//t1.daumcdn.net/brunch/service/user/eUo8/image/s-sLLgpcAaUyFL5YZkzbDjwc1gw.png" %}

**일반적으로 가장 낮은 해상도에서 이미지를 디자인하고, 확대하여 고해상도 에셋(asset)을 만듭니다.** 크기를 조정할 수 있는 벡터 스타일을 사용하는 경우 제어점을 전체 값에 배치하여 1x에서 깔끔하게 정렬되도록 할 수 있습니다. 2x와 3x는 1x의 배수이기 때문에 이 위치 지정을 통해 더 높은 해상도에서 래스터 그리드에 깔끔하게 정렬된 상태를 유지할 수 있습니다.

*   역자설명

    래스터 그리드(raster grid)는 픽셀이 위치해 이미지를 표시하는 행과 열의 그리드입니다.

**각 이미지에 색상 프로필을 제공하세요.** 색상 프로필을 사용하면 앱의 색상이 다양한 디스플레이에서 의도한 대로 표시될 수 있습니다. 지침은 [Color management](https://developer.apple.com/design/human-interface-guidelines/foundations/color/#color-management)를 참고하세요.

**실제 기기에서 이미지를 테스트하세요.** 멋지게 보이는 이미지는 다양한 기기에서 볼 때 픽셀화 되거나 늘어나거나 압축되어 나타날 수 있습니다.



## Platform considerations

_No additional considerations for iOS, iPadOS, macOS, tvOS, or watchOS._

### tvOS

레이어드 이미지는 Apple TV 사용자 경험의 핵심입니다. 계층화된 이미지, 투명도, 크기 조정 및 모션을 결합하여 현실감과 생생한 영상을 사용자에게 제공합니다.

#### Parallax effect

시차 효과(Parallax effect)는 어떤 요소(element)에 초점이 맞춰져 있을 때, 깊이와 역동감을 전달하는 데 사용하는 은은한 시각 효과입니다. 요소(element)에 초점이 맞춰지면 시스템이 요소(element)를 전경으로 올려 부드럽게 흔들면서 요소(element)의 표면이 빛나는 것처럼 보이게 하는 조명을 적용합니다.

이 시차 효과를 위해 레이어 밑의 설명에 나오는 이미지가 필요합니다.

#### Layered images

2\~5개의 서로 다른 레이어가 모여 단일 이미지를 형성하는 것입니다. 투명도를 사용하여 레이어를 분리하고 이를 통해 깊이감을 줍니다. 누군가가 이미지와 상호 작용할 때, 표면에 더 가까운 위쪽 레이어가 올라가고, 크기가 조정된 아래쪽 레이어가 더 멀리 겹쳐져서 3D 효과를 생성합니다.

표준 인터페이스 요소를 사용하여 계층화된 이미지를 표시합니다. 시스템에서 제공하는 [FocusState와](https://developer.apple.com/documentation/swiftui/focusstate) 같은 API 및 표준 보기를 사용하여 계층화된 이미지를 보여줍니다. 계층화된 이미지에 자동으로 시차가 적용됩니다.

tvOS 앱 아이콘은 레이어 이미지를 사용해야 합니다. Top Shelf 이미지를 포함하여 앱에서 초점을 맞출 수 있는 다른 이미지의 경우 계층화된 이미지가 강력히 권장되지만 선택 사항입니다.

*   역자설명

    ‘Top Shelf(상단 선반)’란, 전체 화면 콘텐츠 뷰를 스와이프 하여 예고편과 미리 보기를 재생하고 추가 정보를 얻을 수 있는 뷰에서 상단 뷰를 말합니다.

> 🔥 **IMPORTANT** :  tvOS의 [app icon](https://developer.apple.com/design/human-interface-guidelines/foundations/app-icons)은 레이어 이미지를 사용해야 합니다. [Top Shelf](https://developer.apple.com/design/human-interface-guidelines/components/system-experiences/top-shelf) 이미지를 포함하여 앱에서 초점을 맞출 수 있는 다른 이미지의 경우 계층화된 이미지가 강력히 권장되지만 선택 사항입니다.

**표준 인터페이스 요소를 사용하여 계층화된 이미지를 표시합니다.** [FocusState와](https://developer.apple.com/documentation/swiftui/focusstate) 같은 시스템 제공 포커스 API 및 표준 보기를 사용하는 경우 계층화된 이미지는 사람들이 초점을 맞출 때 자동으로 시차 처리를 받습니다.

**각각의 전경, 중간, 배경 요소를 논리적으로 선택합니다.** 전경 레이어에서 게임의 캐릭터와 같은 눈에 띄는 요소를 표시하거나 앨범 표지 또는 영화 포스터의 텍스트를 표시합니다. 중간 레이어는 2차 콘텐츠 및 그림자와 같은 효과에 적합합니다. 배경 레이어는 전경과 중간 레이어에 집중도를 빼앗지 않고 보여주는 불투명한 배경입니다.

**일반적으로 텍스트를 전경에 두세요.** 텍스트를 가리지 않으려면 명확성을 위해 전경 레이어로 가져와야 합니다.

**배경 레이어를 불투명하게 유지합니다.** 다양한 수준의 불투명도를 사용하는 것은 좋지만, 배경 레이어는 불투명해야 합니다. 그렇지 않으면 아트웍이 시차, 그림자 및 시스템 배경으로 멋지게 보일 수 없습니다.

**레이어링을 단순하고 은은하게 유지해서 보여주세요.** 시차는 거의 눈에 띄지 않도록 디자인됩니다. 과도한 3D 효과는 비현실적이고 거슬리게 보일 수 있습니다. 콘텐츠에 생명을 불어넣고 즐거움을 더하려면 단순하고 은은하게 보여주세요.

**콘텐츠 주변에 안전 구역(safe zone)을 두세요.** 초점 및 시차가 생성되는 시간 동안 일부 레이어의 주변 콘텐츠가 잘리거나 이미지 크기 조정 및 이동으로 인해 명확하게 보기 어려울 수 있습니다. 주요 콘텐츠가 항상 잘 보이도록 하려면 가장자리에 너무 가까이 두지 마세요. 이미지 크기, 레이어 깊이 및 움직임에 따라 안전 영역이 다를 수 있으며 전경 레이어가 배경 레이어보다 더 많이 잘립니다.

{% embed url="https://img1.daumcdn.net/thumb/R1280x0/?fname=http%3A//t1.daumcdn.net/brunch/service/user/eUo8/image/q9_yX7kLWYYYHqSkXiFUb1dylwk.png" %}

**항상 레이어 이미지를 미리 보기 해야 합니다.** Apple TV에서 레이어 된 이미지가 멋지게 보이도록 하려면 Xcode, macOS용 Parallax Previewer 앱 또는 Adobe Photoshop용 Parallax Exporter 플러그인을 사용하여 디자인 프로세스 전반에 걸쳐서 미리 보기를 하는 것이 좋습니다. 크기 조정 및 클리핑이 발생할 때 특별한 주의를 기울이고 필요한 경우 이미지를 다시 조정하여 중요한 콘텐츠를 안전하게 유지하세요. 레이어링 된 이미지가 최종 완성되면 실제 TV에서 미리 보기 하여 사람들이 보게 될 이미지를 확인해 보세요. Parallax Previewer 및 Parallax Exporter를 다운로드하려면 [Resources](https://developer.apple.com/design/resources/#tvos-apps)를 참고하세요.

**초점이 맞지 않은 상태와 초점이 맞춰진 상태를 모두 고려하여 계층화된 이미지에 적합한 크기를 결정합니다.** 시차 효과가 나타날 시간 동안 시스템은 배경 레이어를 약간 자를 수 있으므로 필수 콘텐츠를 안전 영역 내에 유지하고 콘텐츠가 보기 좋게 보이도록 추가 공간을 포함합니다.

{% embed url="https://img1.daumcdn.net/thumb/R1280x0/?fname=http%3A//t1.daumcdn.net/brunch/service/user/eUo8/image/vt8ZRt-gNjBZCRxNhe16qBlmDMM.png" %}

다음 공식은 초점이 맞지 않을 때 이미지의 크기를 기반으로 계층화된 이미지의 크기를 계산하는 데 도움이 될 수 있습니다.

{% embed url="https://img1.daumcdn.net/thumb/R1280x0/?fname=http%3A//t1.daumcdn.net/brunch/service/user/eUo8/image/Hap2X9oeMNKt-s3EAcqtWV-v9rk.png" %}

계층화된 이미지를 앱에 포함하거나, 실행시간 시 콘텐츠 서버에서 검색할 수 있습니다. 앱에 포함할 레이어 이미지를 만들려면 다음 도구 중 하나를 사용하세요.

*   역자설명

    아래 내용은 [Creating Layered Image](https://developer.apple.com/library/archive/documentation/General/Conceptual/AppleTV\_PG/CreatingParallaxArtwork.html) 를 참고하시는 것이 좋습니다.

macOS용 Parallax Previewer 앱. Parallax Previewer는 개별 레이어로 사용할 PNG 파일. lsr, Parallax Exporter 플러그인으로 만든 레이어 이미지(. lsr) 및 레이어 Photoshop 이미지(. psd)를 가져올 수 있습니다. Parallax Previewer는 Xcode 프로젝트로 직접 가져올 수 있는 LSR 파일을 내보낼 수 있습니다.

Parallax Exporter Adobe Photoshop 플러그인. 이 플러그인을 사용하여 Photoshop에서 계층화된 이미지를 테스트하고 Xcode 프로젝트로 직접 가져올 수 있는 LSR 파일로 내보낼 수 있습니다.

엑스코드. 표준 PNG 파일을 앱의 에셋 카탈로그로 드래그하여 Xcode에서 이미지 스택의 개별 레이어 역할을 합니다. 이미지 스택은 LSR 파일로 내보낼 수 있습니다. Xcode는 LSR 파일도 가져올 수 있습니다.

앱이 런타임에 콘텐츠 서버에서 계층화된 이미지를 검색하는 경우 해당 이미지를 런타임 계층화된 이미지(. lcr) 형식으로 제공해야 합니다. 런타임 계층 이미지를 직접 만들지 않습니다. layerutilXcode가 제공하는 명령줄 도구를 사용하여 LSR 파일 또는 Photoshop 파일에서 생성합니다. 런타임 계층 이미지는 다운로드를 위한 것이므로 앱에 포함하지 않는 것이 좋습니다.

### watchOS

**일반적으로 이미지 파일을 작게 유지하려면 투명도를 사용하지 않는 것이 좋습니다.** 항상 동일한 단색 배경색으로 이미지를 디자인하는 경우, 이미지에 배경을 포함하는 것이 더 효율적입니다. 그러나 템플릿 이미지 역할을 하는 컴플리케이션 이미지, 메뉴 아이콘 및 기타 인터페이스 아이콘에서는 투명도가 시스템에서 사용하여 색상을 적용할 위치를 결정하기 때문에 투명도가 필요합니다.

**PDF 자동 스케일링을 사용하면 모든 화면 크기에 대해 단일 에셋을 제공할 수 있습니다.** 40mm 및 42mm 화면용 이미지를 2 배율로 디자인하세요. PDF를 로드할 때 WatchKit은 아래 표시된 값을 사용하여 장치의 화면 크기에 따라 이미지 크기를 자동으로 조정합니다.

{% embed url="https://img1.daumcdn.net/thumb/R1280x0/?fname=http%3A//t1.daumcdn.net/brunch/service/user/eUo8/image/vjyt9vENo6lYlGhOTH_pCe01bsg.png" %}



## Resources

#### **Related**

* [Apple Design Resources](https://developer.apple.com/design/resources/)

#### **Developer documentation**

* [UIImageView — UIKit](https://developer.apple.com/documentation/uikit/uiimageview)
* [NSImageView — AppKit](https://developer.apple.com/documentation/appkit/nsimageview/)
* [FocusState — SwiftUI](https://developer.apple.com/documentation/swiftui/focusstate)

#### **Videos**

*   \*\*[Get Started with Display P3\*\* WWDC 2017](https://developer.apple.com/videos/play/wwdc2017/821/)

    ![https://devimages-cdn.apple.com/wwdc-services/images/7/1915/1915\_wide\_250x141\_2x.jpg](https://devimages-cdn.apple.com/wwdc-services/images/7/1915/1915\_wide\_250x141\_2x.jpg)

## Changelog

***

> September 14, 2022 Added specifications for Apple Watch Ultra.
