# Changelog

## 1.0.1

- **修复**: `LV.font.cpp` 中字体加载成功后未设置 `suc = true` 导致返回状态错误
- **修复**: `LV.disp.cpp` 中 `registerDisplay` 的 JSDoc 类型注解更正为 `@param driver:Display`
- **优化**: `CMakeLists.txt` 移除误复制的 Mongoose TLS 宏定义，重命名内部变量避免命名冲突
- **优化**: 注释掉 `idf_component.yml` 中未使用的 `beshell-drv-disp` 依赖
- **新增**: `src/beshell/lv/lvgl.h` 便捷头文件，统一引入 `lv_conf.h` 和 `lvgl.h`

## 1.0.0

- 初始版本，基于 LVGL 9.0.0，提供 BeShell 的 LVGL GUI 封装
