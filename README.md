# Agnes Animation Pipeline

生成式动画单集（S01E01）生产流水线的 ComfyUI 工作流。

## 内容

```
├── workflows/
│   ├── wf_krea2.json         # Krea 角色/场景生成（30 KB）
│   ├── wf_klein9b.json       # Klein 9B 变体（62 KB）
│   └── wf_krea2_nvfp4.json   # NVFP4 量化变体（18 KB）
├── requirements.txt
└── LICENSE
```

每个 `wf_*.json` 都是完整的 ComfyUI 工作流导出，可直接拖入 ComfyUI 加载，
内含节点连接、采样参数、模型引用、Conditioning 结构，可完整复现生成结果（前提模型一致）。

## 依赖

- ComfyUI
- `requirements.txt`
- 模型：随工作流引用的 checkpoint / LoRA 而定，体积原因不在本仓库内

复现性依赖模型版本一致。生成结果与记录不符时，先核对模型 hash。

## 许可

MIT。模型权重与第三方组件遵循各自原有许可。
