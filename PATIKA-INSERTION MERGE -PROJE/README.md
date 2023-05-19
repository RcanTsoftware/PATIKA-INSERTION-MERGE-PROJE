# Merge Sort

<b>Soru 1:</b> [16,21,11,8,12,22] -> Merge Sort

Yukarıdaki dizinin sort türüne göre aşamalarını yazınız.

---
<b>Cevap 1:</b>  Diziyi ikiye böleriz, çıkan dizileri de ikiye böleriz. Elde edilen parçalar 2 veya daha küçük eleman sayısına ulaştıysa dururuz ulaşmadıysa bölmeye devam ederiz. Elde ettiğimiz her bir parçayı kendi içinde sıralarız. Her bölünmüş parçayı sırasına göre birleştiririz. Tek bir bütün olana dek parçaları birleştirmeye devam ederiz. Tek bir bütün olduğunda dizi sıralanmış olacaktır..

<div style="text-align:center; font-weight:bold;"><p>[16,21,11,8,12,22]</p>
<p>[16,21,11]<--->[8,12,22]</p>
<p>[16,21]<--->[11]<--->[8]<--->[12,22]</p>
<p>[16]<--->[21]<--->[11]<--->[8]<--->[12]<--->[22]</p>
<p>[16,21]<--->[8,11]<--->[12,22]</p>
<p>[8,11,16,21]<--->[12,22]</p>
<p>[8,11,12,16,21,22]</p>
</div>

---
<b>Soru 2:</b> Big-O gösterimini yazınız.

---
<b>Cevap 2:</b>

"<em> Merge Sort, bir "böl-ve-fethet" (divide and conquer) algoritmasıdır. Aşağıda Merge Sort'un <span style="font-weight:bold; color:aqua">O(n*logn)</span> zaman karmaşıklığını açıklayan adımları bulabilirsiniz:

1.  Recursive bir fonksiyon olduğu için sürekli kendini çağırarak diziyi hep ikiye bölmektedir. Her bölünmüş  dizinin Merge işlemi için de dizinin uzunluğu olan N işlem yapıldığından zaman karmaşıklığı <b> O(n*logn) </b> olacaktır.

