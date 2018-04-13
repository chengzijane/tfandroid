# tfandroid

ClassifierActivity 结构

java层
Graph
TensorFlowInferenceInterface


# 图片识别流程：
 1. ClassifierActivity.java     -> processImageRGBbytes
 2. TensorFlowImageClassifier.java ->recognizeImage
 3. TensorFlowInferenceInterface.java -> feed
 4. TensorFlowInferenceInterface.java -> run
 5. Session.Runner->run->runHelper
 6. Java_org_tensorflow_Session_run
 7. TF_SessionRun
 8. TF_Run_Helper
 9. DirectSession::Run
 10. ExecutorImpl::RunAsync
 11. ExecutorState(args, this))->RunAsync(std::move(done))
 12. ExecutorState::ScheduleReady
 13. ExecutorState::Process
 
 
 
 
核心基类 OpKernel
