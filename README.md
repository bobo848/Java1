# Java1
pc机模拟程序
# 计192刘利波2019311290
# 实验一 PC机模拟系统
## 一、实验目的
1.熟悉java项目构成  
2.熟悉并练习java项目建包，源程序编写  
3.练习建立java源程序的类，练习属性及方法的编写  
4.练习编写不同的构造方法  
5.练习利用封装控制属性的访问权限  
6.思考并实现源程序对其他private属性的调用  
7.练习调试java程序，加深对java语法的理解  
8.加深对java面向对象编程的理解  
## 二、实验过程
### 实验实现内容：
用类描述计算机中CPU的速度和硬盘的容量。要求Java应用程序有4个类，名字分别是PC、CPU、HardDisk和Test，其中Test是主类
### 具体步骤：
#### 1.CPU类要求：   
（1）getSpeed()返回speed的值  
（2）要求setSpeed(int m)方法将参数m的值赋值给speed    
#### 2.HardDisk类要求：
（1）getAmount()返回amount的值    
（2）要求setAmount(int m)方法将参数m的值赋值给amount  
#### 3.PC类要求：
（1）setCPU(CPU c)将参数c的值赋值给cpu  
（2）要求setHardDisk(HardDisk h)方法将参数h的值赋值给HD  
（3）要求show()方法能显示cpu的速度和硬盘的容量  
#### 4.主类Test要求：
（1） main方法中创建一个CPU对象cpu，cpu将自己的speed设置为2200；   
（2） main方法中创建一个HardDisk对象disk，disk将自己的amount设置为200；   
（3） main方法中创建一个PC对象pc；   
（4） pc调用setCPU(CPU c)方法，调用时实参是cpu；   
（5） pc调用setHardDisk(HardDisk h)方法，调用时实参是disk；  
（6） pc调用show()方法；  
## 三、核心方法
（1）cpu  
public void setSpeed(int m) {  
	if(m>1000 && m<3000)  
	speed=m;  
    else   
    	{System.out.println("CPU speed was wrong!");  
    	speed=m;  
    	}  
}  
（2）Hardisk  
public int getAmount() {  
	return amount;  
}  
public void setAmount(int amount) {  

    this.amount = amount;  

 }  
 （3）pc 
 public void setCPU(CPU c) {  
	cpu=c;  
}  
void setHardDisk(HardDisk h) {  
	HD=h;  
}  
（4）Test  
public class Test {  

   public static void main(String args[]) {  

       CPU cpu = new CPU(20,"Intel",4.0);  

       HardDisk HD=new HardDisk(512,600);  

       PC pc =new PC(cpu,HD);  

       pc.show();  

    }  

}  
## 四、实验结果
### ![实验结果](https://github.com/bobo848/Java1/blob/main/%E5%AE%9E%E9%AA%8C2%E8%BF%90%E8%A1%8C%E7%BB%93%E6%9E%9C%E6%88%AA%E5%9B%BE.JPG)
## 五、实验感想
通过本次实验，我第一次系统的编写了java源程序并放在项目于包中使其正常运行。熟悉并练习了类及属性与方法的编写，不同构造方法的编写，属性的访问权限的设置及其合理调用。
练习了程序的查错调试。加深了对java面向对象编程的理解。
 
 
 
 
 
 
 
 
 
 
 
