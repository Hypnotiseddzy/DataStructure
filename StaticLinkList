package com.dzy;

public class LinkNode{
    final int N=100010;
    int head;
    int[] e=new int[N];//储存每个节点的元素值
    int[] ne=new int[N];//储存每个节点的下一节点的索引
    int idx;//储存当前数组e的储存位置（到哪一个节点）
    public void init(){
        head=-1;
        idx=0;
    }

    /**
     * 在链表的头节点插入元素
     * @param x 元素的值
     */
    public void add_to_head(int x){
        e[idx]=x;
        ne[idx]=head;
        head=idx;
        idx++;
    }

    /**
     * 将x插入到下标为k的节点后
     * @param k 要插入的位置
     * @param x 要插入的元素值
     */
    public void add(int k,int x){
        e[idx]=x;
        ne[idx]=ne[k];
        ne[k]=idx;
        idx++;
    }

    /**
     * 将下标为k的节点删除
     * @param k 节点索引
     */
    public void remove(int k){
        ne[k]=ne[ne[k]];
    }

    /**
     * 删除头节点
     */
    public void remove_head(){
        head=ne[head];
    }
}


