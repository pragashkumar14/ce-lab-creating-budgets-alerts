# Budget Alert Flow

## Notification Sequence
1. **50% Actual** → Email: "You've used half your $50 monthly budget"
2. **80% Actual** → Email: "Warning — approaching budget limit ($40 of $50 spent)"
3. **100% Forecasted** → Email: "Forecast indicates you will exceed your budget this month"
4. **100% Actual** → Email + Action: deny policy applied to `developers` group

## Response Procedures
- **50%**: Review spending in Cost Explorer, check for unexpected services
- **80%**: Identify top cost drivers, consider stopping non-essential resources
- **100% Forecast**: Immediately audit running resources, stop anything unnecessary
- **100% Actual + Action**: New resource creation blocked; contact team lead to review and lift restriction
