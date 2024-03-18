Grok-1
这个仓库包含了用于加载和运行 Grok-1 开放权重模型的 JAX 示例代码。

请确保下载检查点并将 ckpt-0 目录放在 checkpoint 文件夹中。然后运行以下命令：

pip install -r requirements.txt
python run.py

以测试代码。

该脚本会加载检查点并从模型中对测试输入进行采样。

由于模型的规模较大（3140亿参数），测试模型需要具备足够的GPU内存。此外，此仓库中的 MoE 层的实现并不高效，但为了验证模型的正确性，我们选择了这种实现方式，避免了需要自定义内核的情况。

下载权重
你可以使用种子下载工具下载权重，使用以下链接：

magnet:?xt=urn:btih:5f96d43576e3d386c9ba65b883210a393b68210e&tr=https%3A%2F%2Facademictorrents.com%2Fannounce.php&tr=udp%3A%2F%2Ftracker.coppersurfer.tk%3A6969&tr=udp%3A%2F%2Ftracker.opentrackr.org%3A1337%2Fannounce

许可证
此发布中的代码和相关的 Grok-1 权重受到 Apache 2.0 许可证的约束。该许可证仅适用于此仓库中的源文件和 Grok-1 的模型权重。
