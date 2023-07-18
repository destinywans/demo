apiVersion: v1
kind: Service
metadata:
  name: resource-management
  namespace: dev
  labels:
    app: resource-management
spec:
  type: ClusterIP
  selector:
    app: resource-management
  ports:
    - name: http
      port: 9500
      targetPort: 9500
