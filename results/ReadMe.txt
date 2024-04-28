The file folder name is self-explained. For example, 'Customers_25-Machines_1-Production_Time_Type-M' means that every instance in the folder has 25 customers, one machine mounted on the vehicle, and the type M of production time. The last node is the depot.

The content in the file is output as a solution class.
public class Solution {

    private boolean isFeasible;

    private double objValue;

    private List<ValRoute> routes;

    private List<Integer> unvisitedCustomerIds;

    private double routeCost;
}

public class ValRoute {

    private double value;

    private List<Integer> visitedSequence;

    private List<MachineSchedule> productionSequence;

    private double routeCost;
}

public class MachineSchedule {

    private int machineId;

    private List<Integer> jobIds;

    private double completionTime;
}