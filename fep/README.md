# FEP — FlagOS Enhancement Proposal

## 什么是 FEP

FEP 是 FlagOS 的 Feature 管理机制。每个跨模块或较大 Feature 对应一个 FEP —— 一份 markdown 设计文档，存放在 `fep/sig-*/` 目录下，通过 PR 提交、review、迭代和合入。

**工具链**：GitHub PR + Markdown 文件 + OWNERS 审批

## SIG 分组

| SIG | 覆盖模块 |
|-----|---------|
| `sig-operator` | FlagGems, FlagAttention, FlagFFT, FlagSparse, FlagDNN, FlagBLAS, FlagTensor, FlagAudio |
| `sig-compiler` | FlagTree |
| `sig-network` | FlagCX |
| `sig-framework` | PyTorch-Plugin-FL, vllm-plugin-FL, sglang-plugin-FL, TransformerEngine-FL, Megatron-LM-FL, verl-FL |
| `sig-training` | FlagScale |
| `sig-kernelgen` | KernelGen |
| `sig-embodied` | FlagOS-Robo |
| `sig-ai4s` | FlagQuantum |
| `sig-benchmark` | FlagPerf |
| `sig-skills` | Skills |
| `sig-tools` | FlagRelease |
| `sig-edge` |   — Arm CPU,  NPU, IoT   |
| `sig-architecture` |   Feature  |

##   FEP

|   |  FEP  |
|------|-----------|
|    Feature | ** ** |
|     | ** ** |
|   /  | ** ** |
|      | ** ** |
|     Feature / Bugfix |   |
|     |   |

## FEP  

```
Provisional ──→ Implementable ──→ Implemented
     │                                ↑
     ├──→ Deferred ──────────────────┘
     └──→ Rejected
```

|   |   |   |
|------|------|------|
| **Provisional** |   SIG    |     |
| **Implementable** |     | SIG   approve PR     |
| **Implemented** |     |       |
| **Deferred** |       |      |
| **Rejected** |   |   |

> ** **：FEP    `**Status:**`    ，     PR   。

##  

### 0.   SIG  

  FEP  ，   SIG       。        。

### 1.     

  `fep-template/README.md`  `fep/sig-xxx/title-slug.md`。

- `title-slug`         `-`  
-   ：Summary + Motivation   ，         
-  ** `Provisional`**

### 2.   PR

    PR    。

-   ：    **    **
-     `FEP`  
-   **Draft PR**      

### 3.     

PR    review、 、 。

- SIG   （OWNERS  ）    **approve**  
-       `Implementable`
-  PR      

**  **：  Feature     SIG，   `sig-architecture`  。    SIG   FEP，       SIG   OWNERS     。

### 4.  

-      PR       
-     `Related PRs`   
-         

### 5.  

-         PR    
-       `Implemented`
-         PR   

##  

|   |   |
|------|------|
| `title-slug.md` |   PR   |
| `NNNN-title-slug.md` |  PR    NNNN   |

>  PR      PR    。  PR        。

##  

|   |   |
|------|------|
| **FEP Owner** |   FEP、    、  、  |
| **SIG  **（OWNERS） | Review   approve FEP    |
| **Release Manager** |       FEP  、Go/No-Go   |

## Milestone  

-   FlagOS       Milestone（  `FlagOS 2.1`）
- Milestone    deadline
-       FEP    Milestone
- Release Manager   Milestone      
