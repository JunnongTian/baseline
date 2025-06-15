bash 
conda activate /data/zoujj/anaconda3/envs/gcl
# 设置远程仓库为 SSH
git remote set-url origin git@github.com:JunnongTian/baseline.git
关联仓库
git remote add origin https://github.com/JunnongTian/baseline.git
#更新仓库
git push -u origin master
#可更换参数 --train_dataset  --test_dataset  --task --lr --dropout --use_bn --act_fn --src_dst_agg --num_hops

vim script_name.sh  # 创建 Shell 脚本
i  # 进入插入模式（在光标前插入）
esc保存 :wq退出

运行脚本
chmod +x filename.sh
bash filename.sh

################TMUX##########################
tmux new -s experiment 创建新会话
#运行
# 进入您的项目目录
cd /path/to/your/project

# 运行您的实验脚本
./run_experiments.sh

按 Ctrl+B 然后按 D分离会话程序在后台跑

tmux attach -t experiment 重新连接会话

关闭会话：
# 在会话内部输入
exit

# 或从外部终止
tmux kill-session -t experiment

数据比对
https://m50l8ciihr.feishu.cn/docx/WcGMd7GnDo2xi1xVIRPcviXfnQx


CirGps 可调参数--attn aropout  --local gnn type"  --num heads
 
