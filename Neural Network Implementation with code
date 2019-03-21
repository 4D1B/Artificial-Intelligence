/*
 * To change this license header, choose License Headers in Project Properties.
 * To change this template file, choose Tools | Templates
 * and open the template in the editor.
 */
package javaapplication4;

import static java.lang.Math.exp;

/**
 *
 * @author ADG
 */
public class JavaApplication4 {

    /**
     * @param args the command line arguments
     */
    
    public static float net(float[] i,float[] w,float[] b)
    {
        float net=w[0]*i[0]+ w[1]*i[1] + b[0]*1;
        
        
        
        return net;
    }
    
    public static float net2(float[] i,float[] w,float[] b)
    {
        float net2=w[2]*i[0]+ w[3]*i[1] + b[0]*1;
        
        
        
        return net2;
    }
    
    
    @SuppressWarnings("empty-statement")
    public static void main(String[] args) {

            
            float[] i = {0.05f, 0.10f};
            float[] h = {0.0f,0.0f,0.0f,0.0f} ;
            float[] o = {0.0f,0.0f,0.0f,0.0f} ;
            float[] w = {.15f , .20f, .25f , .30f ,.4f , .45f ,.5f,.55f};
            float[] b = {.35f , .60f};
            float neth1= net(i,w,b);
            
            float outh1=0;
            outh1= (float) (1/(1+exp(-neth1)));
            System.out.println(outh1);
            h[0] = outh1;
            float neth2= net2(i,w,b);
            float outh2 = (float) (1/(1+exp(-neth2)));
            System.out.println(outh2);
            h[1] = outh2;
            float net1 = w[4] * outh1 + w[5] * outh2 + b[1]*1;
            System.out.println(net1);
            
            float out1 = (float) (1/(1+exp(-net1)));
            o[0]= out1;
            float net2 = w[6] * outh1 + w[7] * outh2 + b[1]*1;
            float out2 = (float) (1/(1+exp(-net2)));
            o[1] = out2;
            System.out.println(out2);
            int j=0;
            float[] e= {0.0f,0.0f,0.0f,0.0f} ;
            float[] t={0.01f,0.99f};
            for( j=0;j<2;j++)
            {
                
                e[j]=(float) (0.5*Math.pow((t[0] - o[0]), 2));
            }
            
            System.out.println(e[0] +e[1]);
    }
    
}


