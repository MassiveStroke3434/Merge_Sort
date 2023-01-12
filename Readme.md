<!-- This Merge_Sort project prepared direction of yazilimakademisi lessons -->

Initial List = [16,21,11,8,12,22] -> Merge Sort

1-) "Yukarıdaki dizinin sort türüne göre aşamalarını yazınız."
    On First step; We need to split the list middle of the length until arrived to alone for each component
        [16,21,11,8,12,22]  --> [16,21,11] , [8,12,22] --> [16,21],[11],[8,12],[22] --> [16],[21],[11],[8],[12],[22]

    Second step; we start to merge the components, we need to follow like lowest one positioned on left side when we are merging. We are starting to mergening with double by double 
        [16],[21],[11],[8],[12],[22] --> [16] [21] 16 is lower than 21 so 16 needs to be stay on left --> [16,21]
        [16],[21],[11],[8],[12],[22] --> [11] [8] 8 is lower than 11 so 8 needs to be positioned on left --> [8,11]
        [16],[21],[11],[8],[12],[22] --> [12] [22] 12 is lower than 22 so 12 needs to be stay on left --> [12,22]

        [16,21],[8,11],[12,22] after that we start to compare the value between list, this action happened for left values first after that passing over one left

        for first check; from first list left side value: [16] second list left side value: [8] --> 8 lower than 16, so 8 needs to be on left
        second check; from first list 16 still lower one, second list right side value: [11] --> 11 lower than 16, so 11 needs to be on left
        third check; this check left list done so its direclty went to right --> [8,11,16,21],[12,22]

        we start to do samething between these two list: [8,11,16,21],[12,22]
         from left list first value is: 8, from second list first value:12, 8 is lower than 12, so 8 needs to be stay on left
         from left list second value is:11 from second list first value:12, 11 lower than 12, so 11 needs to be stay on left
         from left list third value is: 16 from second list first value:12, 12 lower than 16, so 12 needs to be stay on left
         from left list third value is: 16 from second list second value:22 16 lower than 22, so 16 needs to be stay on left
         from left list fourth value is:21 from second list second value:22 21 lower than 22, so 21 needs to be stay on left

         to sum up for all theses actions, list will be like; [8,11,12,16,21,22]

2-) "Big-O gösterimini yazınız."
    The Big-O represent like: 2^x = n --> logn --> O(nlogn)



