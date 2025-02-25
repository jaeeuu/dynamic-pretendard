# dynamic-pretendard

dynamic-pretendard is an enhanced dynamic subset font built on the popular [Pretendard](https://github.com/orioncactus/pretendard) base. It tackles the challenge of oversized CSS files common in traditional dynamic subsetting—often seen in implementations by Google—by intelligently optimizing Unicode ranges and CSS payload.

## Overview

Standard dynamic subset solutions leverage machine learning to generate CSS covering extensive Unicode ranges, which often leads to unnecessarily large file sizes.
dynamic-pretendard, however, adopts a data-driven approach using Korean character frequency insights to fine-tune these ranges, thereby achieving a lighter, faster-loading CSS without compromising on quality.
| Type | Size of CSS | Number of files |
|-|:-|:-|
| *Original Pretendard dynamic subset* | 540.4KB | 920 |
| *Original Pretendard Variable dynamic subset* | 52.3KB | 92 |
| *Dynamic-Pretendard* | 19.5KB | 18 |


## Usage

You can use it with
```css
html, body{
  font-family: 'Pretendard', 'Pretendard-fb';
}

```

## Features

- **Optimized CSS Delivery**: Dramatically reduces CSS file size by including only essential character subsets.
- **Data-Driven Subsetting**: Utilizes machine learning-based Korean character rankings to precisely tailor Unicode ranges.
- **Fallback Font for Pretendard**: Implements a refined fallback mechanism that replaces the local Arial font with a version enhanced through custom font metrics. This ensures consistent typography across diverse environments while mitigating cumulative layout shifts (CLS).
- **Built on Pretendard**: Inherits the robust design and versatility of the well-established Pretendard font.

## Note

사용자의 입력값을 표시하는 용도로 적합하지 않습니다.

## License

dynamic-pretendard is derived from the Pretendard font, which is distributed under the SIL Open Font License. To maintain consistency with its base, dynamic-pretendard is also released under the SIL Open Font License.  
For full license details, please see the [LICENSE](LICENSE) file.

## Acknowledgements

- [Pretendard](https://github.com/orioncactus/pretendard) by orioncactus – for providing the excellent base font under the SIL Open Font License.
- [Fontaine](https://github.com/unjs/fontaine) – for inspiring innovative approaches to font optimization.
- [Google's research](https://www.tdcommons.org/dpubs_series/906/) on Korean character frequency and dynamic subsetting – – for motivating a more efficient, data-driven solution.
