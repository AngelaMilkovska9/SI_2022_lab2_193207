Angela Milkovska 193207

import org.junit.jupiter.api.Test;

import java.util.ArrayList;
import java.util.Arrays;
import java.util.List;

import static org.junit.jupiter.api.Assertions.*;

class lab2_siTest {
    private <T> List<String> newArrayList(List<T> asList) {
        return  new ArrayList<>(Arrays.asList());
    }
    @Test
    void everyStatementsTest(){
        IllegalArgumentException lp;

       //1
        lp= assertThrows(IllegalArgumentException.class, () ->SI_lab2.function(newArrayList(Arrays.asList())));
        assertTrue(lp.getMessage().contains("List length should be greater than 0"));

        //2
        lp= assertThrows(IllegalArgumentException.class, () ->SI_lab2.function(new ArrayList(Arrays.asList("0", "0", "0","0", "0"))));
        assertTrue(lp.getMessage().contains("List length should be a perfect square"));

        //3
        assertEquals((new ArrayList<String>(Arrays.asList("1", "#", "2", "0", "3", "#", "1", "#", "#"))),SI_lab2.function(new ArrayList<String>(Arrays.asList("0", "#", "0", "0", "0", "#", "0", "#", "#"))));
    }


}
  
  На цртежот има 45 јазли и 52 ребра. Од 52-45=7. 7+2=9
Комплексноста е 9
  
  Void everystatementsTest{} IllegalArgumentExceptions ex; ex=assertsThrows(IllegalArgumentExceptions.classes, () ->lab2_si.funciton 
(newArrayList(Array.asList()));assertTrue(Ex.getMessage().contains("List lenght should be greater than 0"));ex-assertThrows(IllegalArgumentException
.class()->lab2_si.function(new ArrayList (ArraysList("22',"45","99","65","0")))).assertTrue(ex.getMessage()contains("List lenght should be a perfect
square"))). Prviot test treba da ja sodrzi dolzinata na nizata koja so treba da bide i spored toa kodot frla isklucok i tuka zavrsuva. Dodeka pak vo vtoriot
slucaj gi dodeluvame/stavame brojot na elementi i tie broevi treba da se neparni za da zavrsi programata. I moze da kazeme deka i dvata testa se 
uspesno pominati
