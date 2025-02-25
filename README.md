# dynamic-pretendard

dynamic-pretendard is an improved dynamic subset font built upon the popular [Pretendard](https://github.com/orioncactus/pretendard) font. This project addresses the issue of excessively large CSS file sizes used in traditional dynamic subset implementations, such as those by Google, by optimizing the dynamic subsetting process.

## Overview

Traditional dynamic subset fonts use machine learning to generate a CSS file that covers all required Unicode ranges, often resulting in bulky files. In contrast, dynamic-pretendard:
- Leverages Google's machine learning-based Korean character frequency rankings.
- Fine-tunes the Unicode ranges.
- Reduces the CSS file size for better performance and faster load times.

This streamlined approach ensures that only the necessary characters are loaded, improving efficiency without sacrificing quality.

## Features

- **Optimized CSS File**: Significant reduction in file size compared to conventional methods.
- **Intelligent Subsetting**: Utilizes data-driven character ranking for precise Unicode range adjustments.
- **Foundation on Pretendard**: Inherits the quality and versatility of the well-established Pretendard font.
- **Fallback Font Override**: Overrides local Arial fonts with a custom fallback fontFamily for consistent typography across environments.

## License

dynamic-pretendard is based on the Pretendard font, which is distributed under the SIL Open Font License. To remain consistent with its source, dynamic-pretendard is also released under the SIL Open Font License.  
For full license details, please see the [LICENSE](LICENSE) file.

## Acknowledgements

- [Pretendard](https://github.com/orioncactus/pretendard) by orioncactus – for the excellent base font and its SIL Open Font License.
- [Fontaine](https://github.com/unjs/fontaine) – for inspiring font optimization approaches.
- [Google's research](https://www.tdcommons.org/dpubs_series/906/) on Korean character frequency and dynamic subsetting – for inspiring this more efficient approach.
