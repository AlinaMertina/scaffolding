# Generateclasse
ny nomtable = nomclasse izay ho forinona
ny premierligne misi ny chemin ametrana azy

exemple de tamplate
/home/mertina/Bureau/L3/S5/DAO/nomtable.java     ligne:0 nomtable ilay nom table any anaty base
package etu002087.entity;

import java.util.HashMap;
import java.util.Vector;
import java.sql.*;
import java.text.SimpleDateFormat;
import java.util.Collections;
import java.util.Comparator;
import java.util.Date; 

import generaliser.AmethodeSet;
import generaliser.Generaliser; 
import generaliser.ANomTable; 
import generaliser.Adatabase; 
import generaliser.AmethodeGet; 
import generaliser.APrimarykey; 

import etu002087.framework.Urlannotation; 
import etu002087.framework.ModelView; 
import etu002087.framework.Scopeannotation; 
import etu002087.framework.Set_value_jspannotation; 
import etu002087.framework.Sessionannotation; 
import etu002087.framework.Gsonannotation;

@ANomTable(nomtable = "nomT", nbrclonne =nbrC,nomsequence = "nomS")        reto juste zavatra ilaiko amn le framework Naina
@Adatabase(nombase = "nomB", typebase= "baseT",nomuser= "nomU",password= "passW",port="porT") 
public class nomtable extends Generaliser { 
    public nomtable(){
        super();  
        super.setchild(this);  
    }

    attribu

    primaryKey
    @Set_value_jspannotation(nom_atribue= "Colonne") 
    @AmethodeSet(nomcolonne =  "Colonne")  
    public void setmaxCol(Type Colonne){
        if(Colonne==null){ 
            this.Colonne=super.newprimarykey().toUpperCase(); 
        }else{ 
            this.Colonne=Colonne;
        } 
    }
    @AmethodeGet(nomcolonne ="Colonne") 
    @APrimarykey(nomprimarykey = "Colonne") 
    public Type getmaxCol(){
        return Colonne;
    } 
    finprimaryKey

    debutC
    @Set_value_jspannotation(nom_atribue= "Colonne") 
    @AmethodeSet(nomcolonne =  "Colonne")  
    public void setmaxCol( Type Colonne){
        this.Colonne=Colonne;
    }

    @AmethodeGet(nomcolonne ="Colonne") 
    public Type getmaxCol(){
        return this.Colonne;
    }
    finC

}



