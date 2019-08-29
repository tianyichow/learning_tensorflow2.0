# @tf.function 

- 将python函数编译成图
- 将模型到处成为GraphDef+checkpoint或者SaveModel
- 使得eager execution可以默认打开
- 1.0代码发通过tf.funciton来继续在2.0使用
    * 代替session
    
# API列表

- 基础数据类型
    * tf.constant.tf.string
    * tf.ragged.constant,tf.SparseTensor, tf.Variable
- 自定义损失函数
    * tf.reduce_mean
- 自定义层次
    * keras.layers.Lambda
- tf.function
    * tf.function tf.autograph.to_code,get_concrete_function
  
- GraphDef
    * get_operations, get_peration_by_name
    * get_tensor_by_name, as_graph_def
- 自动求导
    * tf.GradientTape
    * Optimizer.apply_gradients
    
    


- RaggedTensor:2.0新增特性，就是不等长的tensor


#tf.function 