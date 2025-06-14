---

# OCR Character Detection with Tesseract and OpenCV

Этот проект демонстрирует использование библиотеки [Tesseract OCR](https://github.com/tesseract-ocr/tesseract) совместно с [OpenCV](https://opencv.org/) и `pytesseract` для распознавания текста и символов на изображениях. Он также содержит примеры работы с веб-камерой и захватом экрана.

## Возможности

* Распознавание текста из изображения (OCR).
* Визуализация распознанных **символов** с использованием координат (bounding boxes).
* (опционально, закомментировано) Распознавание **слов** с уровнями доверия.
* (опционально, закомментировано) Распознавание **только цифр**.
* (опционально, закомментировано) Распознавание текста в **веб-камере** или **захваченном экране** в реальном времени.

## Зависимости

* Python 3.x
* [OpenCV](https://pypi.org/project/opencv-python/)
* [Pytesseract](https://pypi.org/project/pytesseract/)
* [Pillow](https://pypi.org/project/Pillow/)
* Установленный [Tesseract OCR](https://github.com/tesseract-ocr/tesseract)

## Установка

1. Установите зависимости:

```bash
pip install opencv-python pytesseract Pillow
```

2. Установите [Tesseract OCR](https://github.com/tesseract-ocr/tesseract) и пропишите путь в коде:

```python
pytesseract.pytesseract.tesseract_cmd = 'C:\\Program Files\\Tesseract-OCR\\tesseract.exe'
```

## Использование

1. **Распознавание текста с изображения**

Скрипт загружает изображение `psm.PNG`, распознаёт символы и отображает bounding boxes на экране.

```python
img = cv2.imread('psm.PNG')
# Обработка и отображение результатов
```

2. **Дополнительные функции (опционально):**

* Распознавание **слов** с указанием уровня confidence.
* Распознавание **только цифр**.
* Захват изображения с **веб-камеры** или **экрана** с распознаванием в реальном времени.

