# Daily Mood - Onboarding UI 🎃
<h2>🎯 Descripción del Proyecto: 
 ✅ 🚀 App de diario emocional con un onboarding interactivo de 7 pantallas que guía al usuario desde el registro hasta la personalización de su experiencia emocional.
  </h2>

## 🎯 Efectos Visuales Implementados - 7 pantallas animadas siguiendo Apple HIG:

### 1. **Scale on Selection** (Escala en Selección)
- **Técnica**: `.scaleEffect()` + `.animation(.spring())`
- **Uso**: EmotionChip aumenta 5% al seleccionarse
- **Código**: `scaleEffect(isSelected ? 1.05 : 1.0)`

### 2. **Opacity Fill Transition** (Transición de Opacidad)
- **Técnica**: Fill condicional con opacidad
- **Uso**: Fondo cambia de 20% opacidad a 100% al seleccionar
- **Código**: `.fill(isSelected ? color : color.opacity(0.2))`

### 3. **Spring Animation** (Animación con Resorte)
- **Técnica**: `.animation(.spring(), value:)`
- **Uso**: Transiciones suaves con efecto bounce en toda la UI
- **Código**: `.animation(.spring(), value: isSelected)`

### 4. **Brightness Press Effect** (Brillo al Presionar)
- **Técnica**: ButtonStyle personalizado con `.brightness()`
- **Uso**: +30% brillo momentáneo al presionar botones
- **Código**: `.brightness(configuration.isPressed ? 0.3 : 0)`

### 5. **Rotation Entrance Animation** (Rotación de Entrada)
- **Técnica**: `.rotationEffect()` + `withAnimation`
- **Uso**: Elementos giran 180° al aparecer en pantalla
- **Código**: `.rotationEffect(.degrees(animate ? 0 : 180))`

### 6. **Linear Gradient Background** (Fondo Degradado)
- **Técnica**: `LinearGradient` + `.background()`
- **Uso**: Botones con gradiente dinámico según página activa
- **Código**: `LinearGradient(colors: [color, color.opacity(0.7)])`

### 7. **Selection Border Indicator** (Indicador de Borde)
- **Técnica**: `.stroke()` condicional
- **Uso**: Borde blanco de 2px en elementos seleccionados
- **Código**: `.stroke(isSelected ? Color.white : Color.clear)`

## 🛠 Stack Técnico
- **Framework**: SwiftUI
- **Animaciones**: Spring, EaseInOut, EaseOut
- **Estado**: @State, @Binding, @ObservedObject
- **Layout**: LazyVGrid, TabView, ScrollView


<div class="Galeria">
<img width="400" height="720" alt="Captura de Pantalla 2026-07-02 a la(s) 13 40 14" src="https://github.com/user-attachments/assets/ec9108a7-edd4-45e5-99b5-d1977528deda" />
<img width="400" height="720" alt="Captura de Pantalla 2026-07-02 a la(s) 13 40 39" src="https://github.com/user-attachments/assets/0018e021-5231-4da6-9386-e722acaf2252" />
<img width="400" height="720" alt="Captura de Pantalla 2026-07-02 a la(s) 13 40 52" src="https://github.com/user-attachments/assets/22a874d5-8ba7-4b36-afb0-d9bc3cabdf74" />
<img width="380" height="720" alt="Captura de Pantalla 2026-07-02 a la(s) 13 41 03" src="https://github.com/user-attachments/assets/e48c53ff-3200-4c14-b253-e489f4a0d544" />
<img width="360" height="720" alt="Captura de Pantalla 2026-07-02 a la(s) 13 41 33" src="https://github.com/user-attachments/assets/a06b71bf-1cd7-456f-bfc2-dc5356569ea4" />
<img width="360" height="720" alt="Captura de Pantalla 2026-07-02 a la(s) 13 42 01" src="https://github.com/user-attachments/assets/82780557-2eef-408d-a27b-2efebcbbb242" />

</div>
