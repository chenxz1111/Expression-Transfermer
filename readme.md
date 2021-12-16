## Train

```
python main.py [--batch_size] [--epoch] [--num_layers] [--data_set] 
```

## Test

```
python main.py --test_model model_path [--test_data] [--batch_size] [--epoch] [--num_layers] [--data_set] 
```
## CPU

You may train this model on a CPU by deleting all the  `.cuda()` .

## Parameters

You may use these parameters below to obtain the best performance：

|             | num_layers | epoch | batch_size |
| :---------: | :--------: | :---: | :--------: |
|  bool_expr  |    4/5     |  200  |    400     |
|   bin_cmp   |     4      |  200  |    400     |
|   bin_add   |     4      |  200  |    400     |
|   bin_mul   |     4      |  400  |    400     |
| bin_add_mul |            |       |            |
| bitwise_xor |     2      |  200  |    400     |

## Results of test

|           | Baseline | Space | Hint |
| :-------: | :------: | :---: | :--: |
| bool_expr |  76.77%  |       |      |
|  bin_cmp  |  99.30%  |       |      |
|  bin_add  |  99.60%  |       |      |
|bin_mul|94.30%|||
|bin_add_mul||||
|bitwise_xor|99.63%|||

## Results of extra test

|           | Baseline | Space | Hint |
| :-------: | :------: | :---: | :--: |
| bool_expr |  |       |      |
|  bin_cmp  | |       |      |
|  bin_add  |  66.37% |       |      |
|bin_mul|53.36%|||
|bin_add_mul||||
|bitwise_xor|70.85%|||
