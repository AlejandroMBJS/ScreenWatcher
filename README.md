---
# ScreenWatcher

**Autor:** [AlejandroMBJS](https://github.com/AlejandroMBJS)  
**Estado:** En desarrollo 🔧  
**Lenguaje:** Golang  
**Plataformas:** Linux / Windows  
**Licencia:** MIT

---

## 📌 ¿Qué es?

ScreenWatcher es una herramienta multiplataforma escrita en Go que graba la pantalla de forma ofuscada en segundo plano y detecta cuándo un usuario intenta hacer una captura de pantalla. En lugar de permitir que aplicaciones como Microsoft Teams bloqueen la captura, intenta recuperar el frame visible al momento exacto del intento.

> ⚠️ Proyecto experimental. Aún no está confirmado que pueda superar los nuevos bloqueos de Microsoft Teams. El objetivo es explorar huecos técnicos de forma ética y documentada.

---

## 🎯 Objetivos

- Detectar eventos de captura de pantalla (`PrintScreen`, combinaciones específicas).
- Mantener un buffer temporal de video sin guardarlo completo.
- Extraer solo el frame relevante.
- Evitar almacenamiento innecesario o uso intrusivo de recursos.
- Respetar la privacidad del usuario. Todo corre localmente.

---

## 🚫 ¿Es legal?

Sí. La herramienta no vulnera software ni accede a información privada. Solo captura lo que ya está visible en la pantalla del usuario. Es útil para documentación técnica, QA, auditorías visuales y uso personal.

---

## 📦 Compilación

```bash
git clone https://github.com/AlejandroMBJS/screenwatcher.git
cd screenwatcher
go build -o screenwatcher main.go
## 📦 Compilación

```bash
git clone https://github.com/AlejandroMBJS/screenwatcher.git
cd screenwatcher
go build -o screenwatcher main.go
### ✅ `LICENSE` (MIT)

```text
MIT License

Copyright (c) 2025 AlejandroMBJS

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
