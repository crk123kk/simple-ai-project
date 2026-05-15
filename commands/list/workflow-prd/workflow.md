    执行当前 workflow command 的时候，首先会执行 prd，然后根据 prd 的输出执行 task，再根据 task 的输出执行 architecture，最后根据 architecture 的输出执行 implement，最后根据 implement 的输出执行 test，test不通过则返回执行implement，直到 test 通过为止。

    不需要我手动输入确定，ai 按照这个工作流执行到完成需求为止